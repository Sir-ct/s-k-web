<script>
    import Icon from '@iconify/svelte'
    import Header from "../components/Header.svelte";
    import NavLinks from "../components/NavLinks.svelte";
    import HomePage from '../components/HomePage.svelte';
    import InventoryPage from '../components/InventoryPage.svelte';
    import SalesPage from '../components/SalesPage.svelte';
    import PurchasedPage from '../components/PurchasedPage.svelte';

    let location = window.location.pathname
</script>

<main>
    <div>
        <Header />
        <div class="md:flex md:justify-between">
            <div class="md:w-[20%] bg-[#333333] min-h-[100vh] fixed md:absolute">
               <NavLinks link='/' active={location == '/' ? true : false}>
                <Icon icon='mdi:home' />
                <p class="ml-2 font-medium">Home</p>
               </NavLinks>

               <NavLinks link='/inventory' active={location == '/inventory' ? true : false}>
                <Icon icon='ion:menu' />
                <p class="ml-2 font-medium">Inventory</p>
               </NavLinks>

               <NavLinks link='/sales' active={location == '/sales' ? true : false}>
                <Icon icon='ic:baseline-sell' />
                <p class="ml-2 font-medium">Sales</p>
               </NavLinks>
               <NavLinks link='/purchases' active={location == '/purchases' ? true : false}>
                <Icon icon="mdi:invoice-receive" />
                <p class="ml-2 font-medium">Purchases</p>
               </NavLinks>
            </div>

            <div class="w-full md:w-[80%] ml-auto bg-[#DDDDDD] min-h-[100vh]">
                {#if location == '/'}
                    <HomePage />
                {:else if location == '/inventory'}
                    <InventoryPage />
                {:else if location == '/sales'}
                    <SalesPage />
                {:else if location == '/purchases'}
                    <PurchasedPage />
                {/if}
            </div>
        </div>
    </div>
</main>