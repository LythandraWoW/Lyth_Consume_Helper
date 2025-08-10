# Modified version of Akkio's Consume Helper for personal use.

**Version 1.1.3** - Advanced buff and consumable tracking addon for World of Warcraft turtle (1.12)

## 🎉 NEW IN VERSION 1.1.3 - TURTLE WOW CONSUMABLES EXPANSION

### 🌟 **First-Time User Experience**
- **Welcome Window**: Interactive tutorial for new users
- **Quick Settings Access**: One-click button to open main settings panel where all features are accessible
- **User-Friendly Design**: Comprehensive introduction to addon capabilities
- **Optional Display**: "Don't show again" option with manual `/actwelcome` command access

### 🌟 **Massive Content Expansion**
- **20+ New Turtle WoW Consumables**: Complete integration of Turtle WoW-specific consumables from official wiki
- **Enhanced Organization**: Complete reorganization of all consumables into logical, easy-to-navigate categories
- **New Categories Added**: Alcoholic Beverages and Combat Potions for better item organization
- **Data Structure Optimization**: Cleaned up unnecessary fields and improved performance

### 📋 **Complete New Consumables List**

#### **Elixirs & Juju** (New Additions)
- **Elixir of Frost Power** - 30-minute frost damage enhancement
- **Elixir of Greater Intellect** - 20-minute intellect boost  
- **Juju Flurry** - 20-second attack speed enhancement

#### **Special Potions & Consumables** (New Additions)
- **Ground Scorpok Assay** - 1-hour agility enhancement
- **R.O.I.D.S.** - 1-hour strength enhancement
- **Cerebral Cortex Compound** - 1-hour intellect enhancement  
- **Dreamtonic** - 20-minute Spell power enhancement

#### **Food & Drinks** (New Additions)
- **Le Fishe Au Chocolat** - 15-minute 1% dodge and defense
- **Sweet Mountain Berry** - 10-minute stamina food
- **Danonzo's Tel'Abim Medley** - 15-minute haste food
- **Danonzo's Tel'Abim Surprise** - 15-minute ranged attack power food
- **Danonzo's Tel'Abim Delight** - 15-minute spellpower food
- **Gurubashi Gumbo** - 15-minute Reduce damage taken 
- **Dragonbreath Chili** - 10-minute fire proc effect

#### **Alcoholic Beverages** ⭐ NEW CATEGORY
- **Rumsey Rum Black Label** - 15-minute stamina beverage
- **Medivh's Merlot** - 15-minute stamina beverage
- **Medivh's Merlot Blue** - 15-minute spirit beverage

#### **Weapon Enchants** (New Additions)
- **Consecrated Sharpening Stone** - Enhanced sharpening stone for both weapon slots
- **Blessed Wizard Oil** - Enhanced wizard oil for main hand
- **Frost Oil** - Frost damage weapon enchant for both slots

#### **Combat Potions** ⭐ NEW CATEGORY  
- **Nordanaar Herbal Tea** - Instant health/mana restoration
- **Potion of Quickness** - 30-second haste enhancement
- **Mighty Rage Potion** - Instant rage boost

### 🔧 **Enhanced Organization**
- **Logical Categorization**: Items now properly grouped by type and function
- **Optimized Data Structure**: Removed unnecessary buffIcon fields for instant-effect items
- **Complete Item ID Integration**: All new consumables include proper shopping list compatibility
- **Wiki-Verified Data**: All additions sourced and verified from official Turtle WoW wiki

## 🎉 PREVIOUS UPDATES

### Version 1.1.1 - UI Interaction Fix
- **Fixed Keyboard Input Capture**: Resolved issue where addon frames prevented other UI elements (auction house, etc.) from receiving keystrokes
- **Improved Compatibility**: Better interaction with other addons and game UI elements

### � **Smart Shopping List System**
- **Intelligent Shopping Assistant**: New shopping list module accessible via `/actshopping` or `/actshop`
- **Smart Item Detection**: Only shows enabled buffs that are below your configured thresholds
- **Priority-Based Organization**: Items sorted by importance (Flasks → Elixirs → Weapon Enchants → Food → Other)
- **Configurable Thresholds**: Set different minimum amounts for different consumable types
- **Stock Status Monitoring**: Clear "need X more" messaging and "✓ All consumables well stocked!" confirmation

### 🎯 **Tooltip System**
- **Rich WoW-Style Tooltips**: Complete overhaul providing professional game-quality information display
- **Three-Tier Tooltip System**: 
  1. Bag scanning for items in inventory (most accurate)
  2. Rich item/spell tooltips using database IDs (works without items in inventory)
  3. Enhanced custom tooltips with detailed descriptions
- **Complete Item Database**: Added item IDs for all 37+ consumables (flasks, elixirs, food, weapon enchants)
- **Class Buff Intelligence**: Added spell IDs for all 9 class buffs with detailed spell information
- **Rich Information Display**: Shows vendor prices, item descriptions, requirements, mana costs, and spell effects

## Core Features

🎯 **New User Experience** ⭐ NEW
- **Welcome Window**: First-time user onboarding with interactive tutorial
- **Quick Settings Access**: One-click button to open main settings panel
- **Professional Onboarding**: Comprehensive feature overview and setup assistance
- **User Control**: Optional display with manual access via `/actwelcome` command

🎯 **Smart Buff Tracking**
- Visual tracking of buffs, debuffs, and consumables
- Color-coded status indicators (icon color = active, red = missing)
- Real-time item count display from your bags
- Configurable icons per row layout (1-10 icons)
- **Tooltips**: Rich WoW-style tooltips with complete item and spell information
- **Flexible Icon Spacing**: Adjustable from 30-64 pixels (30px = border-to-border placement)
- Automatic countdown timers for consumables with duration tracking

🛒 **Smart Shopping List** ⭐ NEW
- **Intelligent Consumable Shopping**: Track missing consumables for efficient shopping trips
- **Command**: `/actshop` - Opens shopping list window with all missing items
- **Real-time Updates**: Automatically refreshes based on your current buff status and bag contents
- **Comprehensive Coverage**: Shows ALL consumables you're tracking but don't have in bags
- **Professional Interface**: Consistent styling with main addon windows

⚔️ **Weapon Enchant Support**
- Track weapon enchants for main hand and off hand separately
- One-click enchant application with clear instructions
- Visual slot indicators (MH/OH) for easy identification
- Smart detection of equipped weapons
- **Real-time Timer Tracking**: Live countdown using WoW API for precise timing

🎮 **Enhanced User Interface**
- **Reorganized Settings Panel**: Balanced left/right layout with logical grouping
  - Layout Settings (left): Scale, intervals, rows, spacing
  - Display Settings (right): Tooltips, hover functionality
  - Combat Settings (left): Combat-specific options
- Drag-and-drop movable frames with improved visual spacing
- Scalable UI (0.5x to 2.0x)
- Draggable minimap button - position anywhere around minimap
- Persistent button positioning (saves between sessions)
- **Improved Timer Positioning**: Better readable placement away from icon edges
- Comprehensive tooltips showing buff status, item counts, and action hints

⚡ **Performance Optimized**
- **Enhanced Buff Tracker System**: Multi-layered cleanup preventing memory leaks
  - Immediate cleanup on buff expiration
  - Periodic maintenance every 30 seconds
  - Prevents stale timer display issues
- Smart caching system for bag scanning
- Efficient update cycles with background optimization
- Combat-aware performance modes
- Minimal memory footprint with automatic cleanup
- Automatic settings migration for updates
- Data corruption recovery systems

🛡️ **Combat Integration**
- Optional UI hiding during combat
- Pause updates in combat for maximum performance
- Automatic resumption after combat ends
- No interference with raid/dungeon performance

## Installation

1. Download the addon files or add the GitHub repository link in Turtle Launcher (when using the launcher, skip step 2)
2. Extract all files to your `Interface/AddOns/` folder
3. Restart World of Warcraft
4. Configure using the minimap button or type `/actsettings` in chat

## Commands

- `/act` - Open buff selection window
- `/actsettings` - Open settings panel
- `/actshop` - Open smart shopping list for missing consumables ⭐ NEW
- `/actwelcome` - Show welcome window with quick start guide ⭐ NEW
- `/actbuffstatus` - Force refresh buff status UI
- `/actreset` - Open reset confirmation dialog

## Configuration

### Tracked Buffs
Use the buff selection window to choose which buffs, consumables, and weapon enchants to track. The addon supports:

- **Class Buffs**: Power Word: Fortitude, Divine Spirit, Arcane Intellect, Mark of the Wild, all Paladin Blessings
- **Flasks**: Flask of the Titans, Flask of Supreme Power, Flask of Distilled Wisdom
- **Elixirs & Potions**: Mongoose, Giants, Superior Defense, Shadow Power, Greater Firepower, Mageblood, Greater Arcane Elixir
- **Turtle WoW Customs**: Dreamshard Elixir, Hardened Mushroom, Power Mushroom
- **Juju & Special**: Juju Might, Juju Power, Winterfall Firewater, Spirit of Zanza, Gift of Arthas
- **Food & Drinks**: Smoked Desert Dumplings, Grilled Squid, Nightfin Soup, Runn Tum Tuber Surprise, Dirge's Kickin' Chimaerok Chops
- **Weapon Enchants**: Dense/Elemental Sharpening Stones, Brilliant Wizard/Mana Oil, Blessed Weapon Coating, Shadowoil, Rogue Poisons
- **Custom Categories**: Organized by buff type for easy selection

### Settings Options
The settings interface is organized into logical sections for easy navigation:

**Layout Settings**
- **UI Scale**: Adjust the size of buff status icons (0.5x - 2.0x)
- **Update Interval**: Control refresh rate (1-60 seconds)
- **Icons Per Row**: Customize layout (1-10 icons per row)
- **Icon Spacing**: Precise spacing control (30-64 pixels)
  - 30px = Border-to-border icon placement
  - Higher values create more spread-out layouts

**Combat Settings**
- **Pause Updates**: Stop UI updates during combat for performance
- **Hide Frame**: Completely hide buff status frame during combat

**Display Settings**
- **Show Tooltips**: Enable/disable detailed tooltips on buff icons
- **Hover to Show**: Make frame visible only when hovering over it
  - **Stability**: Enhanced with robust state management to prevent getting stuck
  - **Debug Support**: Use `/actdebug` to diagnose hover issues, `/acthoverfix` for emergency reset
- **Lock Frame**: Hide background and prevent dragging for minimal UI
  - **Position Persistence**: Frame position is automatically saved when dragging
  - **Lock Preservation**: When locked, frame remembers and restores its custom position
  - **Reload Safety**: Position persists through UI reloads and game restarts

## Usage

1. **Setup**: Click the minimap button to open settings
2. **Configure**: Select which buffs to track in the buff selection window  
3. **Customize**: Drag the minimap button to your preferred position
4. **Monitor**: Watch the buff status frame for missing buffs (red icons)
5. **Action**: Click icons to use consumables or apply enchants
6. **Announce**: Missing raid buffs are automatically announced to group

*Tip: Use `/act` for quick access to buff configuration!*

## Weapon Enchants

The addon provides advanced weapon enchant tracking:

- **Visual Status**: See at a glance which weapons need enchants
- **Smart Application**: Click to automatically prepare enchant items
- **Slot Awareness**: Separate tracking for main hand and off hand
- **Clear Instructions**: Step-by-step guidance for enchant application

## Timer System

The addon features an intelligent dual timer system:

### Smart Timer Display
- **Consumables**: Show countdown timers for items with defined durations (flasks, elixirs, food)
- **Class Buffs**: No timers displayed for raid buffs (Power Word: Fortitude, Divine Spirit, etc.)
- **Duration-Based**: Timers only appear on buffs that have duration values in the database

### Dual Timer Architecture
- **Timestamp Tracking**: Consumables use manual timestamp tracking for accuracy
- **API Integration**: Weapon enchants use `GetWeaponEnchantInfo()` for real-time precision
- **Unified Display**: Both systems use the same time formatting for consistency

## Troubleshooting

### Hover-to-Show Issues
If the frame gets stuck visible or hidden when using hover-to-show mode:

1. **Diagnose the Issue**: Run `/actdebug` to see detailed hover state information
   - Look for "MISMATCH!" in the state analysis
   - Check if hide timer has expired but frame is still visible
2. **Emergency Fix**: Use `/acthoverfix` to immediately reset the hover state
3. **Auto-Recovery**: Latest version (1.1.0+) includes automatic recovery from timer expiry issues
4. **Combat Setting Check**: Ensure issue isn't caused by "Pause UI updates in combat" setting conflict (fixed in 1.1.0+)

### Frame Position Problems
If the frame doesn't remember its position when locked:

1. **Verify Setting**: Ensure "Lock Frame" is enabled in Display Settings
2. **Reload Test**: Try `/reload` to test if position is saved properly
3. **Reset Position**: Unlock frame, move to desired position, then lock again

### General Commands
- `/act` - Open buff selection interface
- `/actsettings` - Open settings panel
- `/actshop` - Open smart shopping list for missing consumables ⭐ NEW  
- `/actdebug` - Comprehensive diagnostic information
- `/acthoverfix` - Reset hover-to-show state
- `/actclear` - Clear buff tracker data
- `/actreset` - Reset all settings to defaults

### Timer Features
- **Real-time Updates**: Timers refresh every second for accurate countdown
- **Smart Filtering**: Only relevant buffs show timer information in tooltips
- **Memory Efficient**: Optimized tracking system with minimal performance impact

## Performance

Optimized for smooth gameplay:

- **Bag Caching**: Reduces repeated bag scans
- **Smart Updates**: Fast visual updates vs. full UI rebuilds
- **Combat Modes**: Reduced activity during encounters
- **Memory Efficient**: Minimal impact on game performance

## Upcoming Features

🚀 **Planned for Future Releases:**
- **🏪 Auction House Integration**: Track and update bought consumables and reflect it directly in UI to keep better track
- **📊 Consumable Analytics**: Track usage patterns and consumption statistics over time
- **🔔 Low Stock Alerts**: Configurable warnings when consumables run low

*Have ideas for new features? Join the discussion on Discord or submit suggestions via GitHub Issues!*

## Support

For issues, suggestions, or contributions:
- GitHub: https://github.com/prodigystudios/Akkio_Consume_Helper
- Discord: akkio (higher chance of response if you use this than github)
- Report bugs via GitHub Issues
- Feature requests welcome

## Changelog

### Version 1.1.3 - 2025-08-06 (TURTLE WOW CONSUMABLES EXPANSION)
**Massive Content Addition - 20+ New Turtle WoW Consumables**
- **Enhanced Database**: Added comprehensive Turtle WoW consumables from official wiki
- **New Categories**: Added "Alcoholic Beverages" and "Combat Potions" sections
- **Complete Reorganization**: Restructured all consumables into logical categories
- **Wiki-Sourced Data**: All new items verified against official Turtle WoW documentation
- **Optimized Integration**: New consumables work seamlessly with shopping list and tooltips
- **Technical**: Enhanced data structure with proper item IDs and duration values
- **Organization**: Items properly categorized by type rather than arbitrary groupings

### Version 1.1.2 - 2025-08-01 (TIMER DRIFT FIX)
**UI Interaction Compatibility Fix**
- **Fixed**: Keyboard input capture issue that prevented other UI elements (auction house, etc.) from receiving keystrokes when addon frames were open
- **Technical**: Removed problematic frame-level EnableKeyboard(true) calls from settings frame, reset confirmation frame, and shopping list frame
- **Preserved**: Essential keyboard input functionality for EditBox text fields (threshold editing)
- **Improved**: Addon frames no longer interfere with global keyboard input to other game interface elements

### Version 1.1.0 - 2025-01-20 (MAJOR UPDATE)
**Smart Shopping List & Enhanced Tooltip System**
- **NEW**: Smart Shopping List Module - Complete shopping assistant for missing consumables
  - **Command**: `/actshop` - Opens dedicated shopping list window
  - **Intelligent Tracking**: Shows all consumables you're tracking but don't have in bags
  - **Real-time Updates**: Automatically refreshes based on buff status and inventory
  - **Interface**: Consistent styling with main addon windows
  - **Smart Integration**: Seamlessly works with existing buff tracking system
- **Enhanced**:Tooltip System - Complete overhaul with three-tier enhancement
  - **WoW-Style Tooltips**: Rich, detailed tooltips with complete spell and item information
  - **Spell Integration**: Added comprehensive spell IDs for all class buffs
  - **Cross-Addon Compatibility**: Resolved conflicts with AtlasLoot and other tooltip addons
  - **Enhanced Information Display**: Shows detailed spell descriptions, reagents, and casting information
  - **Fallback System**: Custom tooltip system ensures information always displays correctly
- **Technical Improvements**: Enhanced data architecture and API compatibility
  - **Spell Database**: Complete spell ID integration (Power Word: Fortitude: 1243, Divine Spirit: 14752, etc.)
  - **Compatibility Fixes**: Resolved "unknown link type" errors with AtlasLoot addon
  - **Code Quality**: Enhanced error handling and cross-addon compatibility
- **UI Consistency**: Shopping list close button matches main settings window behavior
  - **Consistent Experience**: All windows now use identical close button implementation

### Version 1.0.7 - 2025-07-19 (CRITICAL UPDATE #2)
**Fixed Combat Pause Setting Conflicts**
- **CRITICAL**: Fixed "Pause UI updates in combat" setting breaking hover-to-show functionality
- **CRITICAL**: Fixed consumable and weapon enchant timer displays freezing during combat pause
- **Root Cause Found**: Combat events were disabling the entire OnUpdate timer, breaking all timer logic
- **Complete Solution**: Hover-to-show and timer displays now work independently of combat pause settings

### Version 1.0.6 - 2025-07-19 (CRITICAL UPDATE)
**Emergency Fix for Hover-to-Show Timer Issues**
- **CRITICAL**: Fixed frame getting stuck visible when hover timer expires
- **Enhanced**: Improved debug detection for expired timer situations  
- **Recovery**: Automatic frame recovery from timer/state mismatches

### Version 1.0.5 - 2025-07-19
**Frame Position Persistence & Hover-to-Show Stability**
- **Enhanced**: Frame Position Persistence - Lock frame now properly saves and restores position
  - **Automatic Position Saving**: Frame position automatically saved when dragging the frame
  - **Position Restoration**: Saved position restored when reloading UI or restarting game
  - **Lock Frame Enhancement**: When lock frame enabled, frame maintains custom position
  - **Smart Defaults**: New installations start centered, existing users get migration support
- **Fixed**: Hover-to-Show Stability - Comprehensive improvements to prevent frame getting stuck
  - **Race Condition Prevention**: Improved OnEnter/OnLeave event handling prevents hover count drift
  - **State Validation**: Enhanced hide timer logic with double-checking before hiding frame
  - **Boundary Protection**: Prevents hover count from going negative or getting out of sync
- **Added**: Advanced Debug Command - Enhanced `/actdebug` with hover-to-show diagnostics
  - **State Analysis**: Shows current alpha, hover count, hide timer status, and frame visibility
  - **Issue Detection**: Automatically detects when frame is stuck visible or hidden
  - **Troubleshooting Guidance**: Provides specific suggestions when state mismatches detected
- **Added**: Emergency Fix Command - New `/acthoverfix` command to reset stuck hover-to-show state
  - **Instant Recovery**: Immediately resets hover count and hide timers
  - **Safe Reset**: Forces frame to proper hidden state when hover count is 0

### Version 1.0.4 - 2025-01-18
**Enhanced UI Layout & Configuration**
- **Enhanced**: Icon Spacing Configuration - Improved icon layout customization
  - Reduced minimum icon spacing from 20 to 30 pixels for border-to-border icon placement
  - Updated icon spacing range to 30-64 pixels with clear label indication
  - Enhanced validation to ensure proper spacing values within acceptable range
- **Enhanced**: Settings UI Reorganization - Complete overhaul of settings interface layout
  - **Streamlined Layout**: Reorganized from scattered right-side layout to clean left-column organization
  - **Layout Settings** (Left): Scale slider, update interval, icons per row, icon spacing
  - **Combat Settings** (Left): Combat-specific options logically grouped below layout settings
  - **Display Settings** (Left): Tooltips, hover-to-show, lock frame features organized below combat settings
  - **Future-Ready**: Right side now available for expansion of additional settings categories
  - Improved visual organization and user experience with logical grouping flow
- **Enhanced**: Visual Polish - Enhanced spacing and padding throughout the UI
  - Added 2px padding between "Buffs" title and icon grid for better visual separation
  - Improved timer positioning: moved from very top/bottom edges to more readable positions
  - Normal buff timers positioned 8px from top edge
  - Weapon enchant timers positioned 8px from bottom edge for better slot indicator separation
- **Enhanced**: Buff Tracker System - Multi-layered cleanup system preventing memory leaks
  - Immediate cleanup on buff removal for instant response
  - Periodic maintenance cleanup every 30 seconds for stale entries
  - Natural expiration cleanup for consistent state management
  - Prevents stale timer display issues and improves memory efficiency
- **Added**: Lock Frame Feature - Advanced frame locking with minimal UI options
  - Hide background, title bar, and frame border for ultra-minimal appearance
  - Prevent accidental dragging during gameplay
  - Settings checkbox with immediate apply/reset functionality
  - Perfect for users who want maximum screen real estate

### Version 1.0.3 - 2025-01-18
**Smart Timer System & Duration Centralization**
- **Added**: Centralized duration system with all buff durations stored in main data structure
- **Added**: Duration fields to all consumable buffs (flasks: 7200s, elixirs: 3600s, food: 900s)
- **Added**: New Turtle WoW custom consumables (Dreamshard Elixir, Hardened Mushroom, Power Mushroom)
- **Added**: Extended weapon enchant support (Brilliant Oils, Blessed Weapon Coating, Shadowoil, Rogue Poisons)
- **Enhanced**: Smart timer display - timers only appear on buffs with duration values
- **Enhanced**: Weapon enchant timer system with real-time API-based tracking using `GetWeaponEnchantInfo()`
- **Enhanced**: Dual timer architecture (timestamps for consumables, API for weapon enchants)
- **Enhanced**: Tooltip system with duration-based filtering for timer information
- **Fixed**: Timer label rendering optimization - no unnecessary timers for class buffs
- **Refactored**: Duration lookup function to use centralized data instead of separate tables

### Version 1.0.2 - 2025-01-17
**Charged Items & Compatibility Fixes**
- **Fixed**: Critical charged item detection bug (oils, sharpening stones)
- **Fixed**: ShaguTweaks compatibility with custom scroll frame implementation
- **Fixed**: Incorrect buff icons for Gift of Arthas, Prayer of Spirit, Arcane Intellect
- **Added**: Proper handling for WoW Classic's negative count behavior for charged items
- **Enhanced**: Debug command improvements and icon database updates

### Version 1.0.1 - 2025-01-17
**Hover-to-Show Feature**
- **Added**: Hover-to-show feature - frame only visible when hovering buff icons
- **Fixed**: Conditional rebuild system respecting hover-to-show settings
- **Enhanced**: Settings application with immediate response
- **Technical**: Ticker optimization and alpha state management improvements

### Version 1.0.0 - 2025-01-17
**Initial Release**
### Version 1.0.0 - 2025-01-17
**Initial Release**
- **Added**: Complete weapon enchant tracking system for main hand and off hand
- **Added**: Smart caching system with 2-second cache refresh for optimal performance
- **Added**: Dual-update system (fast visual updates + full UI rebuilds)
- **Added**: Combat awareness with optional UI hiding and update pausing
- **Added**: Advanced settings panel with comprehensive configuration options
- **Added**: Color-coded feedback system with professional message styling
- **Added**: Weapon slot indicators (MH/OH labels) for enchant tracking
- **Added**: Minimap integration with draggable button and persistent positioning
- **Added**: Flexible layout with configurable icons per row (1-10)
- **Added**: Scalable interface (0.5x to 2.0x) with UI scaling options
- **Added**: Multiple slash commands (`/act`, `/actsettings`, `/actbuffstatus`, `/actreset`)
- **Added**: Automatic group/raid buff request announcements
- **Added**: Version migration system for seamless updates
- **Added**: Emergency reset function for corrupted settings recovery
- **Added**: Interactive tooltips with comprehensive buff status and action hints
- **Enhanced**: Buff selection UI with improved organization and visual clarity
- **Technical**: Function order resolution, caching architecture, and performance monitoring
- **UI/UX**: Professional blue-gray theme with consistent color coding
- **Compatibility**: Full WoW Classic 1.12 support with character-specific settings

## License

This addon is provided as-is for the Turtle WoW community.

---

*Created by Akkio for Turtle WoW 1.12*
