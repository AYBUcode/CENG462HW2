# CENG462 Game Development - Multiplayer 2D Platformer Assignment

## Overview
This assignment extends the basic 2D platformer with multiplayer functionality using Photon PUN 2. Students will create a networked game that combines traditional platformer mechanics with real-time multiplayer features.

## Technical Requirements

### 1. Photon PUN 2 Integration
Students must implement the following networking components:

1.1. Connection Setup
- Initialize PUN 2 using your Photon App ID
- Implement connection status feedback for players
- Handle connection failures gracefully with appropriate user feedback
- Create necessary manager classes for handling network events

1.2. Lobby System
- Create a main menu scene with the following elements:
  - Nickname input field (saved to PlayerPrefs)
  - Room creation interface with room name input
  - Room listing panel showing available rooms
  - Join room button for each listed room
  - Create room button
  - Player's saved nickname displayed
- Implement automatic room list updates
- Show player count for each room
- Display connection status

1.3. Room Management
- Maximum 4 players per room
- Room state synchronization
- Player list display showing all connected players
- Handle player disconnections gracefully
- Implement proper room leaving functionality
- Synchronize room properties across network

### 2. Platformer Integration

2.1. Player Spawning
- Implement network-aware player spawning system
- Define spawn points for multiplayer matches
- Ensure players spawn at different positions
- Handle late-joining players appropriately

2.2. Player Networking
- Synchronize player movement across network
- Implement network-aware animations
- Handle player physics interactions
- Sync player states (idle, walking, jumping)

2.3. Game State Management
- Synchronize game progress across all players
- Handle scene transitions in multiplayer context
- Implement match state management
- Score or progress tracking for all players

### 3. User Interface Requirements

3.1. Main Menu UI
- Clean, intuitive layout
- Clear feedback for all network operations
- Easy navigation between menu sections
- Proper error messaging for network issues

3.2. In-Game UI
- Display connected players list
- Show player nicknames above characters
- Network status indicator
- Room information display

### 4. Data Persistence

4.1. PlayerPrefs Implementation
- Save player nickname
- Store last used room name
- Remember player preferences
- Handle data loading/saving properly

### Scene Structure
1. Main Menu Scene
   - Login Panel
   - Lobby Panel
   - Room Creation Panel
   - Settings Panel

2. Game Scene
   - Spawn Points Container
   - Network Manager
   - Player Container
   - UI Elements

## Testing Requirements

1. Multiplayer Testing
- Test with minimum 2 players
- Verify synchronization
- Check disconnect handling
- Validate room operations

2. Network Conditions
- Test under various network conditions
- Verify lag compensation
- Check reconnection handling

## Submission Requirements

1. Project Deliverables
- Complete Unity project with PUN 2 integration
- WebGL build
- Documentation of network structure
- Project report including all the details
- Youtube presentation is a must, upload you video as unlisted. Share the link.
- Deliver your all project files and documents via a google drive link

2. Technical Documentation
- Class relationship diagrams
- Implementation details
- Known limitations

## Evaluation Criteria

1. Networking Implementation (40%)
- PUN 2 integration quality
- Synchronization accuracy
- Error handling
- Performance optimization

2. Game Functionality (30%)
- Player movement synchronization
- Animation synchronization
- Spawn point management
- Scene management

3. User Experience (20%)
- UI responsiveness
- Error feedback
- Connection status clarity
- Overall polish

4. Code Quality (10%)
- Architecture
- Documentation
- Best practices
- Performance considerations
