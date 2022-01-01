<script lang="ts">
  import "$lib/styles/global.css";
  import "$lib/styles/tailwind.css";
  import Nav from "$lib/components/nav/Nav.svelte";
  import NavLink from "$lib/components/nav/NavLink.svelte";
  import NavLinkWithDropdown from "$lib/components/nav/NavLinkWithDropdown.svelte";
  import NavDropdownLink from "$lib/components/nav/NavDropdownLink.svelte";
</script>

<Nav>
  <div class="font-serif" slot="logo">
    <a href="/" class="bg-black text-white px-3 py-1 text-2xl"> LOGO </a>
  </div>

  <NavLink link="/">Home</NavLink>

  <NavLinkWithDropdown name="About">
    <NavDropdownLink link="/">About Me</NavDropdownLink>
    <NavDropdownLink link="/">About You</NavDropdownLink>
    <NavDropdownLink link="/">About Us</NavDropdownLink>
  </NavLinkWithDropdown>

  <NavLinkWithDropdown name="Gallery">
    <NavDropdownLink link="/">See Me</NavDropdownLink>
    <NavDropdownLink link="/">See You</NavDropdownLink>
    <NavDropdownLink link="/">See Us</NavDropdownLink>
  </NavLinkWithDropdown>

  <NavLink link="/">Contact</NavLink>
</Nav>

<slot />
