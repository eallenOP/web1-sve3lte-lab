<script>
    import Sidebar from "../../components/Sidebar.svelte";
     let navItems = [
    { text: "Home", href: "/" },
    { text: "Profile image", href: "/profile/profile-pic" },
    { text: "Company details", href: "/profile/company" },
    { text: "My contact details", href: "/profile/contact" },
  ];
</script>
<div class="left-side"><Sidebar {navItems} /></div>
<section>
  <h1>All the profile things</h1>
  <slot />
  <p>Use the navigation sidebar to edit parts of your profile</p>
</section>

<style>
  section {
    border: 1px dashed firebrick;
    background-color: indianred;
  }
  .left-side {
    padding: 1em;
    grid-column: 1 / 2;
    background-color: aliceblue;
  }
</style>
