<template>
  <div class="d-flex flex-column">
<!--    search user -->
    <div class="d-flex p-3 align-items-center position-relative justify-content-between w-100">
      <input type="text" v-model="searchs" @input="Searches" class="form-control r-12 pl-4" placeholder="search or start new chat" style="background: #f0f2f5" />
      <svg viewBox="0 0 24 24" height="24" width="24" preserveAspectRatio="xMidYMid meet" class="position-absolute" version="1.1" x="0px" y="0px" enable-background="new 0 0 24 24" xml:space="preserve">
        <path fill="currentColor" d="M15.009,13.805h-0.636l-0.22-0.219c0.781-0.911,1.256-2.092,1.256-3.386 c0-2.876-2.332-5.207-5.207-5.207c-2.876,0-5.208,2.331-5.208,5.207s2.331,5.208,5.208,5.208c1.293,0,2.474-0.474,3.385-1.255 l0.221,0.22v0.635l4.004,3.999l1.194-1.195L15.009,13.805z M10.201,13.805c-1.991,0-3.605-1.614-3.605-3.605 s1.614-3.605,3.605-3.605s3.605,1.614,3.605,3.605S12.192,13.805,10.201,13.805z"></path></svg>
      <span>
        <svg viewBox="0 0 24 24" height="20" width="20"
             preserveAspectRatio="xMidYMid meet" class="" version="1.1" x="0px" y="0px" enable-background="new 0 0 24 24" xml:space="preserve">
          <path fill="currentColor" d="M10,18.1h4v-2h-4V18.1z M3,6.1v2h18v-2H3z M6,13.1h12v-2H6V13.1z"></path></svg>
      </span>
    </div>
<!--    show user -->
    <template v-for="(user, i) in users">
      <div
        v-if="ShowSearch"
        :key="i"
        class="d-flex p-2 justify-content-between align-items-center pointer UsersSelect">
        <div class="d-flex g8 align-items-center">
          <img :src="user.image" alt=""
               style="width: 50px; height: 50px; border-radius: 50%">
          <div class="d-flex flex-column justify-content-center p-0">
            <span class="f14-400">{{ user.name }}</span>
            <span class="f14-400">{{ user.Message }}</span>
          </div>
        </div>
        <div class="d-flex">
          <p class="f14-400">{{ user.time }}</p>
        </div>
      </div>
    </template>
    <!--    show user -->
    <template v-for="(user, i) in FilterUsers">
      <div
        :key="i"
        class="d-flex p-2 justify-content-between align-items-center pointer UsersSelect">
        <div class="d-flex g8 align-items-center">
          <img :src="user.image" alt=""
               style="width: 50px; height: 50px; border-radius: 50%">
          <div class="d-flex flex-column justify-content-center p-0">
            <span class="f14-400">{{ user.name }}</span>
            <span class="f14-400">{{ user.Message }}</span>
          </div>
        </div>
        <div class="d-flex">
          <p class="f14-400">{{ user.time }}</p>
        </div>
      </div>
    </template>
  </div>
</template>

<script>
export default {
  name: "AllUsers",
  data () {
    return {
      searchs: null,
      ShowSearch: true,
      FilterUsers: [],
      users: [
        {
          name: 'pouria rahimy',
          image: require('@/assets/img/User.jpg'),
          Message: 'salam khobi',
          time: 'yesterday'
        },
        {
          name: '09184095907',
          image: require('@/assets/img/User.jpg'),
          Message: 'سلام خوبی فردا میای کلاس',
          time: 'sunday'
        },
        {
          name: 'پارسا',
          image: require('@/assets/img/User.jpg'),
          Message: 'سلام خوبی فردا میای کلاس',
          time: 'sunday'
        },
        {
          name: 'pouria rahimy',
          image: require('@/assets/img/User.jpg'),
          Message: 'salam khobi',
          time: 'yesterday'
        },
        {
          name: '09184095907',
          image: require('@/assets/img/User.jpg'),
          Message: 'سلام خوبی فردا میای کلاس',
          time: 'sunday'
        },
        {
          name: 'پارسا',
          image: require('@/assets/img/User.jpg'),
          Message: 'سلام خوبی فردا میای کلاس',
          time: 'sunday'
        },
        {
          name: 'pouria rahimy',
          image: require('@/assets/img/User.jpg'),
          Message: 'salam khobi',
          time: 'yesterday'
        },
        {
          name: '09184095907',
          image: require('@/assets/img/User.jpg'),
          Message: 'سلام خوبی فردا میای کلاس',
          time: 'sunday'
        },
        {
          name: 'پارسا',
          image: require('@/assets/img/User.jpg'),
          Message: 'سلام خوبی فردا میای کلاس',
          time: 'sunday'
        },
        {
          name: 'pouria rahimy',
          image: require('@/assets/img/User.jpg'),
          Message: 'salam khobi',
          time: 'yesterday'
        },
        {
          name: '09184095907',
          image: require('@/assets/img/User.jpg'),
          Message: 'سلام خوبی فردا میای کلاس',
          time: 'sunday'
        },
        {
          name: 'پارسا',
          image: require('@/assets/img/User.jpg'),
          Message: 'سلام خوبی فردا میای کلاس',
          time: 'sunday'
        }
      ]
    }
  },
  methods: {
    Searches () {
      this.FilterUsers = this.users.filter(user => user.name.includes(this.searchs))
      console.log(this.searchs)
      this.ShowSearch = false
    }
  }
}
</script>

<style scoped lang="scss">
.UsersSelect:nth-child(1){
  border-top: 1px solid #ececec;;
}
  .UsersSelect{
    border-bottom: 1px solid #ececec;
    &:hover{
      background: #a8cafd;
    }
  }
  .showData{
    display: none !important;
  }
</style>
