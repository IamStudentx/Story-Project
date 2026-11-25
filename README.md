# Dusk to Dawn

## Team Members and Roles

| Team Member | Responsibilities |
|---|---|
| [Your Name] | Story development, project documentation, README, and gameplay planning |
| [Teammate Name] | Story flowchart and branching structure |

## Application Overview

### Story Description

*Dusk to Dawn* is a dark Western-themed interactive browser story inspired by classic outlaw stories and Western games like Red Dead Redemption.

The player takes the role of Randal Scrim, better known by his nickname, "Scrim Scram." He is a young outlaw in his mid-twenties with a quick temper, a quicker draw, and a taste for gambling. He enjoys showing off his revolver skills and secretly carries a second revolver behind his duster coat.

The story begins with a robbery that goes horribly wrong, leaving Scrim as the only survivor of his gang. With nowhere else to go, he makes his way to a nearby Western town called DUSK.

Players can visit several locations around town, including a saloon, doctor's office, and sheriff's office. Each location offers different interactions and opportunities that influence the story.

At the saloon, players can gamble at blackjack or have a drink. Drinking provides an opportunity to meet a woman who can potentially become Scrim's romantic companion. At the doctor's office, players can learn more about the town through conversation or remain silent while receiving treatment. At the sheriff's office, Scrim must decide whether to tell the truth or lie about the robbery.

As the story progresses, Scrim becomes involved in a larger conspiracy surrounding the robbery and the town's sheriff. Depending on the player's decisions, Scrim may eventually take the sheriff's badge through blackmail or violence, or expose the truth and leave town.

Romance is an optional part of the story. If the player chooses to pursue the relationship, the woman becomes Scrim's companion for the remainder of the adventure. Every ending involving the relationship includes a final decision about whether to let her go or attempt to make the relationship work.

### Gameplay and Features

- **Interactive Storytelling:** Players make decisions that determine how the story progresses.
- **Branching Story Paths:** Different decisions lead to different encounters, opportunities, and endings.
- **Town Exploration:** Players can visit the saloon, doctor's office, and sheriff's office.
- **Blackjack:** Players can gamble against the house.
- **Character Interactions:** Conversations reveal information about the town and its residents.
- **Romance:** Players can pursue an optional relationship that continues throughout the story.
- **Player Choices:** Decisions influence how the story unfolds and how characters react.
- **Sheriff Storyline:** Players can take the sheriff's badge through blackmail or violence, or expose the truth and leave town.
- **Multiple Endings:** The story has different outcomes depending on the player's decisions and relationships.

### Rules and Navigation

- Players progress through the story by reading dialogue and selecting available choices.
- Choices determine which scenes and story paths become available.
- The saloon offers two activities: playing blackjack or drinking.
- Drinking allows players to meet a woman and choose whether to speak with her.
- Pursuing the relationship allows the woman to become a companion throughout the rest of the story.
- The doctor's office offers small talk or the option to remain silent while receiving treatment.
- The sheriff's office allows players to tell the truth or lie about the robbery. Both choices eventually reveal the sheriff's secret.
- After uncovering the conspiracy, players must decide whether to blackmail the sheriff, take his badge by force, or expose him.
- If the player pursues romance, the final decision determines whether Scrim lets his companion go or tries to make the relationship work.

## Story Flowchart

The following Mermaid flowchart represents the branching structure of the story, including the opening robbery, town exploration, optional romance, sheriff storyline, and possible endings.
***A PNG OF THIS FLOWCHART WILL BE ADDED TO THE REPOSITORY***

flowchart TD
    A(["START: The Robbery"]) --> B["The Robbery Goes Wrong"]
    B --> C["The Entire Gang Is Killed"]
    C --> D{"What Does Scrim Do?"}

    D -->|"Search the bodies"| E["Search for Money and Evidence"]
    D -->|"Run for his life"| F["Escape Without Looking Back"]

    E --> G["Travel to DUSK"]
    F --> G["Travel to DUSK"]

    G --> H{"Choose a Location"}

    H -->|"Saloon"| I["Enter the Saloon"]
    H -->|"Doctor"| J["Visit the Doctor"]
    H -->|"Sheriff"| K["Visit the Sheriff's Office"]

    I --> L{"Choose an Activity"}
    L -->|"Blackjack"| M["Play Blackjack"]
    L -->|"Drink"| N["Have a Drink"]

    N --> O["Meet a Woman"]
    O --> P{"Talk to Her?"}
    P -->|"Yes"| Q["Begin a Relationship"]
    P -->|"No"| R["Leave Her Alone"]

    J --> S{"Talk to the Doctor?"}
    S -->|"Small Talk"| T["Learn About DUSK"]
    S -->|"Stay Silent"| U["Get Patched Up"]

    K --> V{"Tell the Truth?"}
    V -->|"Yes"| W["Explain What Happened"]
    V -->|"No"| X["Invent a Story"]

    W --> Y["Discover the Sheriff's Secret"]
    X --> Y["Discover the Sheriff's Secret"]

    M --> Z["Continue Exploring DUSK"]
    Q --> Z["Continue Exploring DUSK"]
    R --> Z["Continue Exploring DUSK"]
    T --> Z["Continue Exploring DUSK"]
    U --> Z["Continue Exploring DUSK"]
    Y --> AA["Uncover the Robbery Conspiracy"]
    Z --> AA["Uncover the Robbery Conspiracy"]

    AA --> AB{"What Do You Do About the Sheriff?"}

    AB -->|"Blackmail"| AC["Threaten to Expose His Secret"]
    AB -->|"Violence"| AD["Take the Badge by Force"]
    AB -->|"Expose Him"| AE["Reveal the Truth to DUSK"]

    AC --> AF["Become Sheriff"]
    AD --> AF
    AE --> AG["Leave DUSK as an Outlaw"]

    AF --> AH{"Did Scrim Pursue Romance?"}
    AG --> AH

    AH -->|"Yes"| AI{"What Happens to the Relationship?"}
    AH -->|"No"| AJ(["Ending: Alone"])

    AI -->|"Let Her Go"| AK(["Ending: Separate Paths"])
    AI -->|"Make It Work"| AL(["Ending: Together"])
