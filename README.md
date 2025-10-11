# 🎮 UnderTrail

**A Journey Through the Underground**

UnderTrail is a browser-based retro RPG that combines the classic survival mechanics of *The Oregon Trail* with the combat and mercy system from *Undertale*. Navigate 1200 meters through dangerous caverns, manage your party's resources, and decide whether to fight or show mercy to the monsters you encounter.

🎮 **Play Now:** [under-trail.com](https://under-trail.com)

![UnderTrail Screenshot](https://via.placeholder.com/800x400/000000/00ff00?text=UnderTrail+Screenshot)

---

## 🌟 Features

### Core Gameplay
- **Oregon Trail Mechanics**: Manage food, gold, bullets, and party health as you travel
- **Undertale Combat System**: Fight, Act, or show Mercy to unique enemies
- **Party Management**: Lead a party of 4 customizable characters
- **Profession System**: Choose Banker, Carpenter, or Farmer for different starting resources
- **Determination System**: Your choices affect your determination and the ending you receive

### Unique Mechanics
- **Hunting Minigame**: Classic side-scrolling hunting with arrow keys and spacebar controls
- **Sacrifice System**: Trade party members for distance (requires 30+ determination)
- **Custom Epitaphs**: Choose memorial messages for fallen party members
- **Multiple Endings**: TRUE, NEUTRAL, or HOLLOW ending based on your choices

### Enemies
Meet unique monsters in the Underground:
- 🐸 **Froggit** - An awkward, friendly frog
- 🦋 **Whimsun** - A timid, nervous butterfly
- 👾 **Moldsmal** - A brainless wiggling blob
- 👁️ **Loox** - A judgmental eye (don't pick on them!)
- 🥕 **Vegetoid** - A health-conscious veggie
- 🍕 **Pizzaroni** - A ruthless pizza that shows NO MERCY!

### Special Features
- **Retro Aesthetic**: Green phosphor CRT monitor look
- **8-bit Sound Effects**: Custom chiptune sounds for every action
- **Toast Attack**: Pizzaroni's special 1UP-style attack sound
- **No Installation Required**: Runs entirely in your browser

---

## 🎯 How to Play

### Controls
- **Menu Navigation**: Click buttons to make choices
- **Hunting Minigame**: 
  - Arrow Keys: Move your hunter up/down
  - Spacebar: Shoot
  - Goal: Hunt animals for food before time runs out

### Gameplay Tips
1. **Manage Resources**: Keep food stocked and party members healthy
2. **Choose Wisely**: Fighting gives gold but lowers determination; mercy increases it
3. **Hunt Strategically**: You need 10 bullets to hunt, so don't waste them
4. **Watch Determination**: You need 30+ determination to perform sacrifices
5. **Act First**: Use ACT options to increase mercy chance before trying to spare enemies
6. **Pizzaroni Can't Be Spared**: Some enemies refuse mercy—be prepared to fight!

### Winning Conditions
- **Goal**: Travel 1200 meters to escape the Underground
- **TRUE ENDING**: All 4 party members survive + 70+ determination
- **NEUTRAL ENDING**: At least 2 party members survive
- **HOLLOW ENDING**: Only 1 party member survives

---

## 🚀 Local Development

### Running Locally
```bash
# Clone the repository
git clone https://github.com/mjwade/under-trail.git
cd under-trail

# Open in browser
open index.html
# or
python -m http.server 8000  # Then visit http://localhost:8000
```

### File Structure
```
under-trail/
├── index.html          # Complete game (React + Tailwind)
├── README.md          # This file
├── CHANGELOG.md       # Version history
├── LICENSE            # MIT License
└── .gitignore         # Git ignore file
```

### Tech Stack
- **React 18**: UI framework (loaded via CDN)
- **Tailwind CSS**: Styling (loaded via CDN)
- **Vanilla JavaScript**: Game logic
- **HTML5 Canvas**: Graphics rendering
- **Web Audio API**: Sound effects

---

## 🤝 Contributing

Contributions are welcome! Whether it's bug fixes, new features, or new enemies, feel free to submit a pull request.

### Adding a New Enemy

1. Open `index.html`
2. Find the `enemies` array (around line 90)
3. Add your enemy object:

```javascript
{ 
  name: 'YourEnemy', 
  health: 40, 
  attack: 6,
  ascii: '👻',  // Choose an emoji
  intro: 'Your enemy appears with a spooky message!',
  actOptions: [
    { name: 'Action1', effect: 'mercy', amount: 40, text: 'Result text!' },
    { name: 'Action2', effect: 'mercy', amount: 20, text: 'Another result!' }
  ],
  attacks: [
    'Your enemy does something!',
    'Your enemy attacks differently!'
  ],
  spareText: 'Your enemy is spared!',
  noMercy: false  // Set to true if enemy can't be spared
}
```

4. Test locally
5. Submit a PR!

### Development Guidelines
- Keep all game code in `index.html` for simplicity
- Test in Chrome, Firefox, and Safari before submitting
- Add new features to CHANGELOG.md
- Use descriptive commit messages

---

## 📝 License

MIT License - See [LICENSE](LICENSE) file for details

---

## 🙏 Credits

**Created by**: [mjwade](https://github.com/mjwade)

**Inspired by**:
- *The Oregon Trail* (1971) - MECC
- *Undertale* (2015) - Toby Fox

**Special Thanks**:
- Claude (Anthropic) for development assistance
- The Undertale community for inspiration
- All playtesters and contributors

---

## 📞 Contact & Links

- 🌐 Website: [under-trail.com](https://under-trail.com)
- 🐙 GitHub: [github.com/mjwade/under-trail](https://github.com/mjwade/under-trail)
- 🐛 Report Bugs: [GitHub Issues](https://github.com/mjwade/under-trail/issues)
- 💬 Discussions: [GitHub Discussions](https://github.com/mjwade/under-trail/discussions)

---

## 🎵 Fun Facts

- Pizzaroni's "Toast!" attack plays a 1UP sound from Super Mario Bros
- There are 10 different epitaph choices for sacrificed party members
- The hunting minigame runs at 60 FPS using requestAnimationFrame
- All sound effects are generated in real-time using Web Audio API
- The game contains zero external assets—everything is code!

---

**⭐ If you enjoy UnderTrail, please star the repo!**

Made with ❤️ and determination