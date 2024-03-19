<template>
  <div id="app" class="bg-[#eee9e9] rounded-[16px] p-[20px] shadow-[0_0_12px_rgba(0, 0, 0, 0.1)] flex flex-col justify-center items-center">
    <h1 class="text-[30px] mb-[1.5rem]">Chronomètre</h1>
    <div class="flex flex-col items-center gap-[20px]">
      <div class="timer text-[40px] bg-[#ffffff] p-[20px] rounded-[8px] shadow-[0_0_12px_rgba(0, 0, 0, 0.1)] animate-[pulse_1.5s_infinite_alternate]">
        <span id="minutes">00</span>:
        <span id="seconds">00</span>:
        <span id="milliseconds">00</span>
      </div>
      <div class="flex gap-[1rem]">
        <button id="startBtn">Commencer</button>
        <button id="stopBtn">Arrêter</button>
        <button id="pauseBtn">Pause</button>
        <button id="resetBtn">réinitialiser</button>
      </div>
      <div class="w-[100%]">
        <h2 class="text-[1.5rem]">Lap Timer</h2>
        <ul id="laplist"></ul>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>

  .timer span {
    width: 110px;
    display: inline-block;
    text-align: center;
  }

  button {
    padding: 0.75rem 1.5rem;
    font-size: 1rem;
    text-transform: uppercase;
    font-weight: bold;
    background-color: #f25191;
    color: #ffffff;
    border: none;
    border-radius: 8px;
    cursor: pointer;
    transition: background-color 0.3s ease-in-out;
  }

  button:hover {
    background-color: #d72a76;
  }

  // ul {
  //   list-style-type: none;
  //   padding: 0;
  //   margin: 0;
  //   overflow-y: auto;
  //   max-height: 200px;
  //   background-color: #ffffff;
  //   border-radius: 8px;
  //   box-shadow: 0 0 12px rgba(0, 0, 0, 0.1);
  // }

  // li {
  //   padding: 1rem;
  //   border-bottom: 1px solid #e0e0e0;
  // }

  // li:last-child {
  //   border-bottom: none;
  // }

  // li span {
  //   font-weight: 700;
  // }

</style>