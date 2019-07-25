<template>
  <div>
    <div class="field">
      <label class="label">Name</label>
      <div class="control">
        <input class="input" type="text" placeholder="Please input your name." v-model="name" />
      </div>
    </div>

    <div class="field">
      <label class="label">Email</label>
      <div class="control">
        <input class="input" type="email" placeholder="Please input your Email." v-model="email" />
      </div>
    </div>

    <div class="field">
      <label class="label">Gender</label>
      <div class="control">
        <div class="select">
          <select v-model="gender">
            <option></option>
            <option value="male">male</option>
            <option value="female">female</option>
          </select>
        </div>
      </div>
    </div>

    <div class="field">
      <label class="label">Profile</label>
      <div class="control">
        <textarea class="textarea" placeholder="Max 500 length" v-model="profile"></textarea>
      </div>
    </div>

    <div class="field" v-show="mode == 'create'">
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

<script>
export default {
  props: {
    mode: String // create, update, view
  },
  data() {
    return {
      name: "",
      email: "",
      gender: "",
      profile: ""
    };
  },
  mounted() {
    switch (this.mode) {
      case "crete":
        break;
      case "update":
        this.name = "hoge";
        this.email = "hoge@example.com";
        this.gender = "male";
        this.profile = "This is my profile.";
        break;
      case "view":
        break;
    }
  }
};
</script>
