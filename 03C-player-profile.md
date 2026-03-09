# 03C – Player Profile

The Player is a core entity in the system.

Players belong to **teams**, and teams participate in **competitions or tournaments**.

The system follows a **Fair Play principle**:
- Registration is simple
- Errors can be corrected
- Duplicate profiles can be resolved

---

# Player Architecture

Competition / Tournament  
↓  
Teams  
↓  
Players  

Club  
↓  
Teams  
↓  
Players  

Players **do not join competitions directly**.  
Players participate through teams.

---

# Global Player ID

Each player has a permanent **Global Player ID**.

Rules:

- Created when the player profile is first created
- Never reused
- Never changed
- Remains even if the player changes team or club

Example:

GPID-89347211

---

# Player Minimum Data

The system must allow **lightweight registration**.

Required fields:

- First Name
- Last Name
- Birth Date or Birth Year
- Country

Optional fields:

- Profile Photo
- Preferred Position
- Height
- Weight
- Jersey Number

---

# Player Dashboard

Each player has a personal **dashboard** where they can manage their profile.

Dashboard sections:

1. Profile
2. Teams
3. Competitions / Tournaments
4. Matches
5. Statistics
6. Invitations
7. Privacy Settings
8. Profile Corrections

---

# Parent / Guardian

For minors:

- A parent or guardian can manage the player profile
- A guardian may manage multiple players
- The guardian can approve invitations and privacy settings

---

# Multi-Team Membership

Players may belong to multiple teams depending on rules.

Examples:

- Club team
- School team
- Tournament team

Competition rules may limit participation.

---

# Duplicate Profile Handling

The system does not block registration heavily.

Instead it follows a **Fair Play correction model**:

1. Possible duplicate detected
2. Player / guardian notified
3. Correction requested
4. Time given to respond
5. Club or admin resolves if necessary
6. Profiles may be merged

---

# Player Transfers

Players may move between teams.

Rules:

- Player ID remains
- History remains
- Previous teams are preserved

---

# Player Statistics

Players collect statistics from matches:

- Matches Played
- Goals
- Assists
- Yellow Cards
- Red Cards
- Minutes Played

Statistics are tied to the **Global Player ID**.
