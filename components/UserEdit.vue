<template>
  <div>
    <div class="field">
      <label class="label">Name</label>
      <div class="control">
        <input class="input" type="text" placeholder="Please input your name." />
      </div>
    </div>

    <div class="field">
      <label class="label">Email</label>
      <div class="control">
        <input class="input" type="email" placeholder="Please input your Email." />
      </div>
    </div>

    <div class="field">
      <label class="label">Gender</label>
      <div class="control">
        <div class="select">
          <select>
            <option>male</option>
            <option>female</option>
          </select>
        </div>
      </div>
    </div>

    <div class="field">
      <label class="label">Profile</label>
      <div class="control">
        <textarea class="textarea" placeholder="Max 500 length"></textarea>
      </div>
    </div>

    <div class="field">
      <div class="control">
        <label class="checkbox">
          <input type="checkbox" />
          I agree to the
          <a href="#">terms and conditions</a>
        </label>
      </div>
    </div>

    <div class="field is-grouped">
      <div class="control">
        <button class="button is-link">Submit</button>
      </div>
    </div>
  </div>
</template>
