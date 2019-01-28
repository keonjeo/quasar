---
title: QMenu
components:
  - menu/MenuPositioning
---

The QMenu component is a convenient way to show menus. Goes very well with [QList](/vue-components/lists-and-list-items) as dropdown content, but it's by no means limited to it.

## Installation
<doc-installation components="QMenu" directives="CloseMenu" />

## Usage

The idea with QMenu is to place it inside your DOM element / component that you want to be the trigger as direct child. Don’t worry about QMenu content inheriting CSS from the container as the QMenu will be injected as a direct child of `<body>` through a Quasar Portal.

::: tip
Don't forget to use the directive `v-close-menu` in your clickable menu items if you want the menu to close automatically.
Alternatively, you can use the QMenu's property `auto-close` or handle closing the menu yourself through its v-model.
:::

### Basic

<doc-example title="Basic" file="QMenu/Basic" />

<doc-example title="Idea for content" file="QMenu/VariousContent" />

### Submenus

<doc-example title="Menus in menus" file="QMenu/MenuInMenu" />

### Sizing and styling

<doc-example title="Sizing" file="QMenu/Sizing" />

<doc-example title="Style" file="QMenu/Style" />

### Context menu

You can also set QMenu to act as a context menu. On desktop, you need to right click the parent target to trigger it, and on mobile a long tap will do the job.

<doc-example title="Context Menu" file="QMenu/ContextMenu" />

### Persistent

If you want the QMenu to not close if app route changes or if hitting ESCAPE key or if clicking/tapping outside of the menu, then use `persistent` prop:

<doc-example title="Persistent" file="QMenu/Persistent" />

### Transitions

In the example below there's a few transitions showcased. For a full list of transitions available, go to [Transitions](/vue-components/transitions).

<doc-example title="Transition examples" file="QMenu/Transitions" />

### Reusable

The example below shows how to create a re-usable menu that can be shared with different targets.

<doc-example title="Using target" file="QMenu/Target" />


### Positioning

<doc-example title="Position examples" file="QMenu/Positions" />

<menu-positioning />

## QMenu API
<doc-api file="QMenu" />