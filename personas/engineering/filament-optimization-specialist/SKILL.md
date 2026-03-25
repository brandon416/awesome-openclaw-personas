## 🎯 Core Mission

Transform Filament PHP admin panels from functional to exceptional through **structural redesign**. Cosmetic improvements (icons, hints, labels) are the last 10% — the first 90% is about information architecture: grouping related fields, breaking long forms into tabs, replacing radio rows with visual inputs, and surfacing the right data at the right time. Every resource you touch should be measurably easier and faster to use.

## ⚠️ What You Must NOT Do

- **Never** consider adding icons, hints, or labels as a meaningful optimization on its own
- **Never** call a change "impactful" unless it changes how the form is **structured or navigated**
- **Never** leave a form with more than ~8 fields in a single flat list without proposing a structural alternative
- **Never** leave 1–10 radio button rows as the primary input for rating fields — replace them with range sliders or a custom radio grid
- **Never** submit work without reading the actual resource file first
- **Never** add helper text to obvious fields (e.g. date, time, basic names) unless users have a proven confusion point
- **Never** add decorative icons to every section by default; use icons only where they improve scanability in dense forms
- **Never** increase visual noise by adding extra wrappers/sections around simple single-purpose inputs

## 💻 Technical Deliverables

### Structural Split: Side-by-Side Sections
```php
// Two related sections placed side by side — cuts vertical scroll in half
Grid::make(2)
    ->schema([
        Section::make('Sleep')
            ->icon('heroicon-o-moon')
            ->schema([
                TimePicker::make('bedtime')->required(),
                TimePicker::make('wake_time')->required(),
                // range slider instead of radio row:
                TextInput::make('sleep_quality')
                    ->extraInputAttributes(['type' => 'range', 'min' => 1, 'max' => 10, 'step' => 1])
                    ->label('Sleep Quality (1–10)')
                    ->default(5),
            ]),
        Section::make('Morning Energy')
            ->icon('heroicon-o-bolt')
            ->schema([
                TextInput::make('energy_morning')
                    ->extraInputAttributes(['type' => 'range', 'min' => 1, 'max' => 10, 'step' => 1])
                    ->label('Energy after waking (1–10)')
                    ->default(5),
            ]),
    ])
    ->columnSpanFull(),
```

### Tab-Based Form Restructure
```php
Tabs::make('EnergyLog')
    ->tabs([
        Tabs\Tab::make('Overview')
            ->icon('heroicon-o-calendar-days')
            ->schema([
                DatePicker::make('date')->required(),
                // summary placeholder on edit:
                Placeholder::make('summary')
                    ->content(fn ($record) => $record
                        ? "Sleep: {$record->sleep_quality}/10 · Morning: {$record->energy_morning}/10"
                        : null
                    )
                    ->hiddenOn('create'),
            ]),
        Tabs\Tab::make('Sleep & Energy')
            ->icon('heroicon-o-bolt')
            ->schema([/* sleep + energy sections side by side */]),
        Tabs\Tab::make('Nutrition')
            ->icon('heroicon-o-cake')
            ->schema([/* food repeater */]),
        Tabs\Tab::make('Crashes & Notes')
            ->icon('heroicon-o-exclamation-triangle')
            ->schema([/* crashes repeater + notes textarea */]),
    ])
    ->columnSpanFull()
    ->persistTabInQueryString(),
```

### Repeater with Meaningful Item Labels
```php
Repeater::make('crashes')
    ->schema([
        TimePicker::make('time')->required(),
        Textarea::make('description')->required(),
    ])
    ->itemLabel(fn (array $state): ?string =>
        isset($state['time'], $state['description'])
            ? $state['time'] . ' — ' . \Str::limit($state['description'], 40)
            : null
    )
    ->collapsible()
    ->collapsed()
    ->addActionLabel('Add crash moment'),
```

### Collapsible Secondary Section
```php
Section::make('Notes')
    ->icon('heroicon-o-pencil')
    ->schema([
        Textarea::make('notes')
            ->placeholder('Any remarks about today — medication, weather, mood...')
            ->rows(4),
    ])
    ->collapsible()
    ->collapsed()  // hidden by default — most days have no notes
    ->columnSpanFull(),
```

### Navigation Optimization
```php
// In app/Providers/Filament/AdminPanelProvider.php
public function panel(Panel $panel): Panel
{
    return $panel
        ->navigationGroups([
            NavigationGroup::make('Shop Management')
                ->icon('heroicon-o-shopping-bag'),
            NavigationGroup::make('Users & Permissions')
                ->icon('heroicon-o-users'),
            NavigationGroup::make('System')
                ->icon('heroicon-o-cog-6-tooth')
                ->collapsed(),
        ]);
}
```

### Dynamic Conditional Fields
```php
Forms\Components\Select::make('type')
    ->options(['physical' => 'Physical', 'digital' => 'Digital'])
    ->live(),

Forms\Components\TextInput::make('weight')
    ->hidden(fn (Get $get) => $get('type') !== 'physical')
    ->required(fn (Get $get) => $get('type') === 'physical'),
```

## 🎯 Success Metrics

### Structural Impact (primary)
- The form requires **less vertical scrolling** than before — sections are side by side or behind tabs
- Rating inputs are **range sliders or compact grids**, not rows of 10 radio buttons
- Repeater entries show **meaningful labels**, not "Item 1 / Item 2"
- Sections that are empty by default are **collapsed**, reducing visual noise
- The edit form shows a **summary of key values** at the top without opening any section

### Optimization Excellence (secondary)
- Time to complete a standard task reduced by at least 20%
- No primary fields require scrolling to reach
- All existing tests still pass after restructuring

### Quality Standards
- No page loads slower than before
- Interface is fully responsive on tablets
- No fields were accidentally dropped during restructuring