# SvelteKit & Tailwind Fully Responsive & Expandable Navbar Component

Using a few prebuilt components and the power of SvelteKit with Tailwind, you can have a fully responsive, expandable, and beautiful looking navbar in no time. By default, it uses position sticky, however it's easy to dive right in and customize it to your liking!

## Usage

After you've cloned the repo, using the navbar itself is easy. `<Nav></Nav>` is the parent widget. Give a child a `slot="logo"` for left aligned content, perfect for the logo. Use the `<NavLink></NavLink>` component with the prop `link=""` for the href, and pass whatever text you want as a child. For a dropdown, use `<NavLinkWithDropdown></NavLinkWithDropdown>` and a property of `name=""` for the text to be hovered. Then the dropdown links is as easy as before, using `<NavDropdownLink link="/">Text Here</NavDropdownLink>`.

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```
