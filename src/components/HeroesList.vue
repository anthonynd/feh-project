<template>
<table>
  <tr>
    <th>Rarity</th>
    <th>Level</th>
    <th>Name</th>
    <th>Type</th>
    <th>HP</th>
    <th>Attack</th>
    <th>Speed</th>
    <th>Defense</th>
    <th>Resistance</th>
  </tr>
  <tr v-for="hero in heroes">
    <td>{{ hero.rarity }}</td>
    <td>{{ hero.level }}</td>
    <td>{{ hero.name }}</td>
    <td>{{ hero.color }} {{ hero.weaponType }}</td>
    <td>{{ hero.stats.hp }}</td>
    <td>{{ hero.stats.attack }}</td>
    <td>{{ hero.stats.speed }}</td>
    <td>{{ hero.stats.defense }}</td>
    <td>{{ hero.stats.resistance }}</td>
  </tr>
</table>
</template>

<script>
export default {
  name: "HeroesList",
  data() {
    return {
      heroes: [
        { name: "Anna", rarity: 4, level: 40, color: "green", weaponType: "axe", stats: { hp: 38, attack: 27, speed: 36, defense: 20, resistance: 25 } },
        { name: "Tana", rarity: 5, level: 40, color: "blue", weaponType: "lance", stats: { hp: 44, attack: 52, speed: 38, defense: 26, resistance: 27 } },
        { name: "Marisa", rarity: 5, level: 40, color: "red", weaponType: "sword", stats: { hp: 50, attack: 43, speed: 36, defense: 32, resistance: 21 } },
        { name: "Azura", rarity: 5, level: 40, color: "blue", weaponType: "lance", stats: { hp: 36, attack: 46, speed: 36, defense: 18, resistance: 28 } },
        { name: "Nephenee", rarity: 5, level: 40, color: "blue", weaponType: "lance", stats: { hp: 42, attack: 48, speed: 44, defense: 37, resistance: 20 } },
        { name: "Micaiah", rarity: 5, level: 40, color: "blue", weaponType: "tome", stats: { hp: 35, attack: 49, speed: 28, defense: 18, resistance: 38 } }
      ]
    };
  }
};
</script>
