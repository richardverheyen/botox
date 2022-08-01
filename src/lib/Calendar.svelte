<script>
  let cats = [
		{ name: 'Keyboard Cat' },
		{ name: 'Maru' },
		{ name: 'Henri The Existential Cat' },
		{ name: 'Henri The Existential Cat' },
		{ name: 'Henri The Existential Cat' },
		{ name: 'Henri The Existential Cat' },
		{ name: 'Henri The Existential Cat' },
		{ name: 'Henri The Existential Cat' },
	];
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
  {#each cats as { name }, i}
		<li>
			{i}
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
