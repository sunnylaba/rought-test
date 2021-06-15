<template>
  <div class="row mt-3">
    <div class="col-4">
      <div class="list-group">
        <router-link
          to="/newpage/a"
          class="list-group-item list-group-item-action"
          aria-current="true"
        >
          元件A
        </router-link>
        <router-link
          to="/newpage/b"
          class="list-group-item list-group-item-action"
          aria-current="true"
        >
          元件B
        </router-link>
        <router-link
          to="/newpage/namedView/c2a"
          class="list-group-item list-group-item-action"
          aria-current="true"
        >
          命名路由 c2a
        </router-link>
        <router-link
          to="/newpage/namedView/a2b"
          class="list-group-item list-group-item-action"
          aria-current="true"
        >
          命名路由 a2b
        </router-link>
        <router-link
          to="/newpage/dynamicRoughter/:id"
          class="list-group-item list-group-item-action"
          aria-current="true"
        >
          動態路由
        </router-link>
        <router-link
          to="/newpage/dynamicRouterByProps/:id"
          class="list-group-item list-group-item-action"
          aria-current="true"
        >
          動態路由props
        </router-link>
        <router-link
          to="/newpage/routerNavigation"
          class="list-group-item list-group-item-action"
          aria-current="true"
        >
          路由導覽
        </router-link>
      </div>
    </div>
    <div class="col-8">
      <router-view></router-view>
    </div>
  </div>
</template>
