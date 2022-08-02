<script>
	/**
	 * @type {any}
	 */
   export let rockets = [];
  //  console.log({rockets});
</script>

<ul>
  <li>Mon</li>
  <li>Tue</li>
  <li>Wed</li>
  <li>Thu</li>
  <li>Fri</li>
  <li>Sat</li>
  <li>Sun</li>
</ul>

<ul>
  {#each rockets as { rocket_name }, i}
    <li>
      {rocket_name}
    </li>
  {/each}
</ul>

<style lang="scss">
  ul {
    display: flex;
    flex-wrap: wrap;
    padding-left: 0;

    li {
      box-sizing: border-box;
      list-style: none;
      width: calc(100% / 7);
      height: 80px;
      padding: 4px;
      border: 1px solid black;
      background-color: aquamarine;
    }
  }
</style>
