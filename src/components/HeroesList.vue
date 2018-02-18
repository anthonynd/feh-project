<template>
</template>

<script>
  export default {
    name: 'HeroesList',
    data() {
      return {
        heroes: [
          {
            name: 'Anna',
            rarity: 4,
            level: 40,
            stats: {
              hp: 38,
              attack: 27,
              speed: 36,
              defense: 20,
              resisitance: 25
            },
            weapon: {
              name: 'Silver Axe',
              might: 11
            },
            skills: {
              a: null,
              b: 'Vantage 2',
              c: 'Spur Res 3'
            }
          }
        ]
      }
    }
  }
</script>