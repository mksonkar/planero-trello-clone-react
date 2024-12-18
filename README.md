# Planero - A Trello-inspired Project Management App

Watch the demo on YouTube: 

[![Watch the demo video](https://img.youtube.com/vi/PsPuVJGiQ_w/hqdefault.jpg)](https://www.youtube.com/watch?v=PsPuVJGiQ_w)

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Getting Started](#getting-started)
   - [Prerequisites](#prerequisites)
   - [Installation](#installation)
5. [Usage](#usage)
   - [Creating Boards](#creating-boards)
   - [Managing Lists](#managing-lists)
   - [Manipulating Cards](#manipulating-cards)
   - [Drag and Drop Functionality](#drag-and-drop-functionality)
6. [Project Structure](#project-structure)
7. [Future Enhancements](#future-enhancements)
8. [Contributing](#contributing)
9. [License](#license)

## Introduction

Planero is a Trello-inspired project management application built using React and Tailwind CSS. It provides a user-friendly interface for organizing tasks, managing projects, and collaborating with team members. The app allows users to create boards, lists, and cards to visualize their workflow and stay on top of their tasks.

## Features

- Create, edit, and delete boards
- Add, reorder, and delete lists within a board
- Create, edit, and delete cards within a list
- Drag and drop functionality to rearrange lists and cards
- Persistent data with localStorage
- Responsive design for seamless usage across devices

## Technologies Used

- **React**: A JavaScript library for building user interfaces
- **Tailwind CSS**: A utility-first CSS framework for rapidly building custom designs
- **Hello Pangea DnD**: A powerful drag and drop library for React
- **UUID**: A library for generating unique identifiers
- **React Icons**: A collection of popular icon sets in React

## Getting Started

<details>
  <summary>Steps to replicate project locally:</summary>
### Prerequisites

- Node.js (version 14 or higher)
- npm (version 6 or higher)

### Installation

1. Clone the repository:

```bash
git clone https://github.com/raknos13/planero-trello-clone-react.git
```

2. Navigate to the project directory:

```bash
cd planero-trello-clone-react
```

3. Install the dependencies:

```bash
npm install
```

4. Start the development server:

```bash
npm run dev
```

The app will be available at `http://localhost:3001`

</details>

## Usage

### Creating Boards

To create a new board, click the "+" button in the sidebar and enter a title and color for the board.

### Managing Lists

Within a board, you can add new lists by clicking the "+" button at the end of the list container. Lists can be reordered using the drag and drop functionality.

### Manipulating Cards

Each list can contain multiple cards. You can add new cards, edit their titles, and move them between lists using drag and drop.

### Drag and Drop Functionality

The app utilizes the [hello-Pangea/DnD](https://github.com/hello-pangea/dnd) library to provide seamless drag and drop functionality. Users can rearrange lists and cards by clicking and dragging them to the desired position.

## Project Structure

<details>
  <summary>
The project's codebase is organized as follows:
  </summary>

```
├── src
│   ├── assets
│   │   ├── not-found-alt.svg
│   │   └── not-found.svg
│   ├── components
│   │   ├── Board
│   │   │   ├── AddNew.jsx
│   │   │   ├── Board.jsx
│   │   │   ├── Card.jsx
│   │   │   ├── EmptyBoard.jsx
│   │   │   ├── index.js
│   │   │   └── List.jsx
│   │   ├── shared
│   │   │   ├── AutoResizeTextarea.jsx
│   │   │   ├── BoardCreatorPopover.jsx
│   │   │   ├── ConfirmPopover.jsx
│   │   │   ├── DarkModeToggle.jsx
│   │   │   ├── GithubButton.jsx
│   │   │   ├── index.js
│   │   │   └── MoreOptionsPopover.jsx
│   │   ├── Sidebar
│   │   │   ├── BoardList.jsx
│   │   │   ├── index.js
│   │   │   ├── SidebarCollapsed.jsx
│   │   │   ├── SidebarHeader.jsx
│   │   │   └── Sidebar.jsx
│   │   ├── Header.jsx
│   │   ├── index.js
│   │   └── Main.jsx
│   ├── contexts
│   │   ├── BoardContext.jsx
│   │   ├── index.js
│   │   ├── SidebarContext.jsx
│   │   └── ThemeContext.jsx
│   ├── hooks
│   │   ├── useLocalStorage.js
│   │   └── useTasks.js
│   ├── App.css
│   ├── App.jsx
│   ├── index.css
│   ├── initialData.js
│   ├── main.jsx
│   └── TODOS_FOR_PROJECT.md
├── eslint.config.js
├── index.html
├── package.json
├── package-lock.json
├── postcss.config.js
├── README.md
├── tailwind.config.js
└── vite.config.js
```

</details>

The `components` directory contains the main UI components of the application, such as the Board, List, and Card components and the `shared` directory inside `components` holds reusable UI components and utilities. The `contexts` directory houses all state management logic,
Each directory has an `index.js` barrel file to simplify imports in the project.

## Future Enhancements

These are the TODOS for the project as of now. Not in any priority order.

> See the issues section to see features I'm working on currently

- [x] Implement dark theme and theme switching
- [x] Add local storage for persistent data
- [ ] Implement user authentication and authorization
- [ ] Implement a landing page
- [ ] Add the ability to assign labels to cards
- [ ] Integrate with third-party services (e.g., Google Calendar, Slack)
- [ ] Develop a mobile-optimized version of the application

## Contributing

Contributions to the Planero project are welcome! If you have any ideas, bug reports, or feature requests, please feel free to open an issue or submit a pull request. Make sure to follow the project's coding conventions and test your changes before submitting a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
