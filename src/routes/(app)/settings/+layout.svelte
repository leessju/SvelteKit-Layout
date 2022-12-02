<script>
    import "../../../app.postcss";
    export let data;
</script>

<div class="drawer drawer-mobile">
    <input id="my-drawer-2" type="checkbox" class="drawer-toggle" />
    <div class="drawer-content flex flex-col p-8">
      <!-- Page content here -->
      <slot />
      <label for="my-drawer-2" class="btn btn-primary drawer-button lg:hidden">Open drawer</label>
    
    </div> 
    <div class="drawer-side border-r-2">
      <label for="my-drawer-2" class="drawer-overlay"></label> 
      <ul class="menu p-4 w-80 bg-base-100 text-base-content">
        <!-- Sidebar content here -->
        <li><a href="/settings">Main Settings</a></li>
        <li><a href="/settings/appearance">Appearance</a></li>
        <li><a href="/settings/profile">Profile <b>{data.user.email}</b></a></li>
      </ul>
    
    </div>
  </div>

