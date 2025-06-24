# GAS\_Template Wiki

**GAS\_Template** is a production-ready, modular, and data-driven Gameplay Ability System (GAS) framework for Unreal Engine, heavily inspired by the architecture of Epic Games' **Lyra Starter Game**.

This project is designed to serve as a lightweight and scalable alternative to Lyra, retaining its key systems—such as Ability Sets, Input Configuration, and Pawn Data—while offering a simplified foundation tailored for quick integration into any GAS-based Unreal project.

---

## 🔧 Core Features

* **Data-Driven Gameplay Architecture**
* **Gameplay Ability System (GAS) Integrated**
* **Enhanced Input System Support**
* **Modular Ability Sets**
* **Attribute Sets and Effects**
* **Tag-Based Activation**
* **Blueprint and C++ Compatible**

---

## 🧩 Included Gameplay Examples

This template includes a range of plug-and-play gameplay abilities:

* 🏃 **Sprint Ability** – Increases movement speed while sprinting.
* 🛷 **Adaptive Sliding** – Initiates a sliding movement that dynamically responds to terrain slope.
* 🩸 **Dynamic Falling Damage** – Applies damage based on landing velocity and fall height.
* 💀 **Death System** – Handles actor death state, including ability cancellation and state transition.
* ⬆️ **Jump / Double Jump** – Standard and multi-jump functionality using GAS.

Each ability is powered by GAS and activated via gameplay tags defined in the Enhanced Input system.

---

## 🧠 System Overview

### PawnData

Defines what a pawn can do: abilities, input config, attribute sets, and camera mode. Enables fully data-driven character setup.

### Ability Sets

Grouped data assets that define which Gameplay Abilities, Effects, and Attribute Sets a character should have. Automatically granted at runtime.

### Input Config

Maps input actions to gameplay tags using Enhanced Input. Enables tag-based ability activation without manual bindings.

### Gameplay Effects

Reusable effects for modifying attributes (e.g., sprint speed, mana cost, cooldowns, falling damage). Fully configurable and tag-driven.

---

## 🚀 Getting Started

1. Enable required plugins:

   * GameplayAbilities
   * GameplayTasks
   * GameplayTags
   * Enhanced Input

2. Create or configure your Pawn using `PawnData`.

3. Assign `AbilitySets` and input configs in `PawnData`.

4. Set up your player controller and character blueprint to use GAS components.

---

## 🔄 Lyra Compatibility

GAS\_Template shares the same structural approach as Lyra. If you're familiar with Lyra’s:

* `PawnData`
* `InputConfig`
* `AbilitySystemComponent`
* `AbilitySet`

...then you'll feel right at home. Most Lyra documentation and learning resources apply directly to this template.

---

## 📂 Project Structure

* `Core/`: Base C++ classes (Character, Controller, PawnData, Abilities)
* `Abilities/`: Predefined GAS abilities and effects
* `Input/`: Enhanced Input configs and mappings
* `UI/`: Optional HUD or UI elements for displaying cooldowns, mana, etc.
* `Data/`: Ability sets, attribute sets, tags

---

## 📘 Documentation Reference

This project uses design conventions aligned with:

* [Lyra Starter Game Documentation](https://dev.epicgames.com/documentation/en-us/unreal-engine/lyra-sample-game-in-unreal-engine?application_version=5.0)
* [Unreal GAS Documentation](https://github.com/tranek/GASDocumentation)

---

For developers who want a modular and scalable GAS foundation without the full overhead of Lyra, **GAS\_Template** provides a clean, extensible solution.
