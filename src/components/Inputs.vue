<template>
  <div class="input-wrapper">
    <div class="inputs">
      <form action="">
        <label class="form-control">
          <input type="radio" name="radio" />
          Radio
        </label>

        <label class="form-control">
          <input type="radio" name="radio" checked />
          Radio - checked
        </label>
      </form>
    </div>
    <div class="inverted-label">
      <label class="input">
        <span class="input-label">Text Input</span>
        <input class="input-field" type="text" />
      </label>
    </div>

    <div class="select">
      <label class="select-label">Selection</label>
      <select name="" id="">
        <option value="op-1">Option 1</option>
        <option value="op-2">Option 2</option>
        <option value="op-3">Option 3</option>
      </select>
    </div>
  </div>
</template>
<style scoped>
:root {
  --select-border: #777;
  --select-focus: blue;
  --select-arrow: var(--select-border);
}
.input-wrapper {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-evenly;
}
.select-label {
  color: black;
  text-align: left;
}
select {
  appearance: none;
  background-color: transparent;
  border: none;
  margin: 0;
  padding: 0 1rem 0 0;
  margin: 0;
  width: 100%;
  font-family: "Righteous", sans-serif;
  font-size: inherit;
  cursor: inherit;
  line-height: inherit;

  outline: none;
}
option {
  box-shadow: 0 0 0.2rem #fff, 0 0 0.2rem #fff, 0 0 2rem #bc13fe,
    0 0 0.8rem #bc13fe, 0 0 2.8rem #bc13fe, inset 0 0 1.3rem #bc13fe;
}
.select {
  width: 100%;
  margin-top: 0;
  margin-bottom: 4rem;
  min-width: 15ch;
  max-width: 30ch;
  border: 1px solid var(--select-border);
  border-radius: 0.25em;
  padding: 0.25em 0.5em;
  font-size: 1.25rem;
  cursor: pointer;
  line-height: 1.1;
  background: rgba(226, 226, 226, 0.8);

  box-shadow: 0 0 0.2rem #fff, 0 0 0.2rem #fff, 0 0 2rem #bc13fe,
    0 0 0.8rem #bc13fe, 0 0 2.8rem #bc13fe, inset 0 0 1.3rem #bc13fe;
}
.select::after {
  content: "";
  width: 0.8em;
  height: 0.5em;
  background-color: var(--select-arrow);
  clip-path: polygon(100% 0%, 0 0%, 50% 100%);
}
.form-control {
  font-size: 2rem;
  font-weight: bold;
  line-height: 1.1;
  display: grid;
  grid-template-columns: 1em auto;
  gap: 0.5em;
}
.inputs {
  width: 50%;
  text-align: left;
  margin: 2rem;
  margin-top: 0;
}
.neon-text {
  color: #fff;
  font-family: "Sacramento", sans-serif;
  text-shadow: 0 0 7px #fff, 0 0 10px #fff, 0 0 21px #fff, 0 0 42px #bc13fe,
    0 0 82px #bc13fe, 0 0 92px #bc13fe, 0 0 102px #bc13fe, 0 0 151px #bc13fe;
  font-size: 3.2rem;
}
.inverted-label {
  margin: auto;
}
.input {
  font-size: 2rem;
  font-weight: bold;
}
.input-label {
  position: absolute;
  top: 41rem;
  z-index: 3;
}
label {
  font-family: "Righteous", sans-serif;
  color: #fff;
}
input[type="radio"] {
  box-shadow: 0 0 0.2rem #fff, 0 0 0.2rem #fff, 0 0 2rem #bc13fe,
    0 0 0.8rem #bc13fe, 0 0 2.8rem #bc13fe, inset 0 0 1.3rem #bc13fe;
  margin: 0;
  border-radius: 50%;
  width: 2em;
  height: 2em;
  appearance: none;
  border: 0.15rem solid #fff;
  display: grid;
  place-content: center;
  transform: translateY(-0.075em);
}
input[type="radio"]::before {
  width: 2.5em;
  height: 2.5em;
  content: "";
  border-radius: 75%;
  transform: scale(0);
  transition: 120ms transform ease-in-out;
  box-shadow: inset 1em 1em #f5e1fd;
}
input[type="radio"]:checked::before {
  transform: scale(0.5);
}
input[type="text"] {
  background: rgba(226, 226, 226, 0.8);
  border: none;
  box-shadow: 0 0 0.2rem #fff, 0 0 0.2rem #fff, 0 0 2rem #bc13fe,
    0 0 0.8rem #bc13fe, 0 0 2.8rem #bc13fe, inset 0 0 1.3rem #bc13fe;
  border-radius: 0.5rem;
  border: none;
  position: relative;
  line-height: 2rem;
  width: 15rem;
  font-family: "Righteous", sans-serif;
  font-size: 1.5rem;
}
</style>