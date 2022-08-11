<template>
  <div class="buttons">
    <button class="submit">Submit</button>
    <button class="confirm">Confirm</button>
    <button class="warning">Warning</button>
    <button class="error">Error</button>
  </div>
</template>

<style>
button {
  margin: 1rem;
  cursor: pointer;
  padding: 0.5rem;
  font-family: "Righteous", sans-serif;
  font-size: 2rem;
  color: #fff;
  background-color: rgba(255, 255, 255, 0.5);
  box-shadow: 0 0 0.2rem #fff, 0 0 0.2rem #fff, 0 0 2rem #bc13fe,
    0 0 0.8rem #bc13fe, 0 0 2.8rem #bc13fe, inset 0 0 1.3rem #bc13fe;
  border-radius: 2rem;
  border: none;
}

.submit:hover {
  box-shadow: 0 0 0.2rem #fff, 0 0 0.2rem #fff, 0 0 2rem #2313fe,
    0 0 0.8rem #2313fe, 0 0 2.8rem #2313fe, inset 0 0 1.3rem #2313fe;
}

.confirm:hover {
  box-shadow: 0 0 0.2rem #fff, 0 0 0.2rem #fff, 0 0 2rem #13fe4e,
    0 0 0.8rem #13fe4e, 0 0 2.8rem #13fe4e, inset 0 0 1.3rem #13fe4e;
}

.warning:hover {
  box-shadow: 0 0 0.2rem #fff, 0 0 0.2rem #fff, 0 0 2rem #fea013,
    0 0 0.8rem #fea013, 0 0 2.8rem #fea013, inset 0 0 1.3rem #fea013;
}

.error:hover {
  box-shadow: 0 0 0.2rem #fff, 0 0 0.2rem #fff, 0 0 2rem #fe1313,
    0 0 0.8rem #fe1313, 0 0 2.8rem #fe1313, inset 0 0 1.3rem #fe1313;
}
</style>