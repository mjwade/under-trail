# Changelog

All notable changes to UnderTrail will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [Unreleased]

### Planned Features
- Save game functionality
- Mobile touch controls optimization
- Additional enemies and bosses
- Achievement system
- Leaderboard integration

---

## [1.0.0] - 2025-01-XX

### 🎉 Initial Release

#### Added - Core Features
- **Complete game loop**: Travel, rest, hunt, and trade mechanics
- **Party system**: Manage 4 customizable party members
- **Profession selection**: Choose between Banker, Carpenter, or Farmer
- **Resource management**: Food, gold, bullets, health, and determination stats
- **Win condition**: Travel 1200 meters to escape the Underground
- **Multiple endings**: TRUE, NEUTRAL, and HOLLOW endings based on performance

#### Added - Combat System
- **Undertale-inspired combat**: FIGHT, ACT, and MERCY options
- **6 unique enemies**: Froggit, Whimsun, Moldsmal, Loox, Vegetoid, and Pizzaroni
- **Enemy-specific ACT options**: Each enemy has 3 unique interaction choices
- **Mercy system**: Build up mercy percentage through ACT choices
- **Determination stat**: Tracks moral choices (fighting vs sparing)

#### Added - Enemies
- 🐸 **Froggit** (30 HP, 5 ATK): Friendly frog who enjoys compliments and jokes
- 🦋 **Whimsun** (20 HP, 3 ATK): Timid butterfly who needs consoling
- 👾 **Moldsmal** (25 HP, 4 ATK): Brainless blob that responds to imitation
- 👁️ **Loox** (35 HP, 6 ATK): Judgmental eye that hates being picked on
- 🥕 **Vegetoid** (40 HP, 5 ATK): Health-conscious veggie that rewards eating greens
- 🍕 **Pizzaroni** (50 HP, 8 ATK): Ruthless pizza with NO MERCY mechanic

#### Added - Special Mechanics
- **Hunting minigame**: Side-scrolling shooter with arrow key controls
  - Hunt rabbits (30 pts), deer (50 pts), and birds (20 pts)
  - 30-second time limit
  - Bullet consumption system (requires 10 bullets to hunt)
  - Real-time collision detection
  - ASCII art animals with smooth animations
- **Sacrifice system**: Trade party members for 300m of distance
  - Requires minimum 30 determination
  - Costs 30 determination points
  - 10 custom epitaph choices
  - Epitaphs displayed on party cards and final stats
- **Random events**: 8 different events that occur during travel
  - Supply chests, friendly monsters, accidents, discoveries
  - Events can affect food, gold, health, or determination

#### Added - Audio System
- **8-bit sound effects** using Web Audio API
- **Unique sounds for each action**:
  - Shooting (sawtooth wave burst)
  - Hitting animals (triangle wave bounce)
  - Fighting (descending sawtooth)
  - ACT menu (ascending sine melody)
  - Mercy/Spare (rising triangle melody)
  - Sacrifice (haunting descending dirge)
  - Pizzaroni's "Toast!" attack (1UP-style melody from Super Mario)
- **Contextual music**: Different themes for title screen and encounters
- **Sound toggle**: Enable/disable sound effects from title screen

#### Added - Visual Design
- **Retro CRT aesthetic**: Green phosphor monitor look with glow effect
- **ASCII art**: Text-based graphics and animations
- **Monospace font**: Authentic retro terminal appearance
- **Canvas rendering**: Smooth animations for travel and hunting screens
- **Responsive UI**: Tailwind CSS styling
- **Color-coded UI elements**:
  - Green: Main UI and living party members
  - Red: Dead party members and danger warnings
  - Yellow: Mercy action and warnings
  - Purple: Sacrifice mechanic
  - Blue: ACT action

#### Added - User Experience
- **Character creation screen**: Name your party and choose profession
- **Party status display**: Real-time HP tracking for all members
- **Game log**: Scrolling event history (last 4 messages)
- **Status indicators**: Day counter, distance progress, resources
- **Button shortcuts**: Keyboard-friendly navigation hints
- **Mobile-friendly**: Responsive design for various screen sizes

#### Technical Details
- **Single-file application**: Entire game in one HTML file
- **No external dependencies**: All libraries loaded via CDN
- **React 18**: Component-based UI architecture
- **Tailwind CSS**: Utility-first styling
- **HTML5 Canvas**: Graphics rendering
- **Web Audio API**: Real-time sound synthesis
- **RequestAnimationFrame**: Smooth 60 FPS animations
- **Ref-based state management**: For hunting minigame performance

---

## Version History

### Version Numbering
- **Major (X.0.0)**: Significant gameplay changes or new game modes
- **Minor (1.X.0)**: New features, enemies, or mechanics
- **Patch (1.0.X)**: Bug fixes, balance changes, and small improvements

---

## [Future Roadmap]

### v1.1.0 - Quality of Life Update
- [ ] Add save/load game functionality
- [ ] Improve mobile touch controls
- [ ] Add settings menu (volume control, difficulty)
- [ ] Balance adjustments based on player feedback

### v1.2.0 - Content Expansion
- [ ] Add 3-5 new enemies
- [ ] Introduce boss battles
- [ ] Add new random events
- [ ] Expand sacrifice system with more epitaphs

### v1.3.0 - Social Features
- [ ] Local leaderboard (browser storage)
- [ ] Achievements system
- [ ] Share results on social media
- [ ] Daily challenge mode

### v2.0.0 - Major Expansion
- [ ] New game modes (Hard mode, Endless mode)
- [ ] Item/Equipment system
- [ ] Branching story paths
- [ ] Multiple Underground zones

---

## Contributing

When contributing, please:
1. Update this CHANGELOG with your changes
2. Use appropriate version numbering
3. Include the date of release
4. Categorize changes as Added, Changed, Fixed, or Removed

For unreleased features, add them under `[Unreleased]` at the top.