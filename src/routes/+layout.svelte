<script>
    import "../style.css";
    import Navbar from "./LayoutComps/Navbar.svelte";
</script>

<Navbar/>
<div class="drawer drawer-end lg:drawer-open overflow-hidden h-full">
    <input id="SideDrawer" type="checkbox" class="drawer-toggle" />
    <div class="drawer-content flex flex-col items-center justify-center w-full h-full">
        <!-- Page content here -->

        <main class="main">
            <slot />
        </main>

    </div>
    <div class="drawer-side w-full">
        <label
            for="SideDrawer"
            aria-label="close sidebar"
            class="drawer-overlay"
        ></label>
        <ul class="menu bg-base-200 text-base-content min-h-full w-80 p-0">
            <!-- Sidebar content here -->
            <li><a>Sidebar Item 1</a></li>
            <li><a>Sidebar Item 2</a></li>
        </ul>
    </div>
</div>

