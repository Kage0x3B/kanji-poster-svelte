<script>
    import {
        Collapse,
        Navbar,
        NavbarToggler,
        NavbarBrand,
        Nav,
        NavItem,
        NavLink
    } from "sveltestrap";

    let isOpen = false;
    const toggleOpen = () => isOpen = !isOpen;
    const updateOpen = e => isOpen = e.detail.isOpen;
</script>

<Navbar color="light" class="shadow-sm" expand="md">
    <NavbarBrand>KanjiPoster</NavbarBrand>
    <NavbarToggler on:click={toggleOpen} />
    <Collapse {isOpen} navbar expand="md" on:update={updateOpen}>
        <Nav class="ml-auto" navbar>
            <NavItem>
                <NavLink>Test</NavLink>
            </NavItem>
        </Nav>
    </Collapse>
</Navbar>
