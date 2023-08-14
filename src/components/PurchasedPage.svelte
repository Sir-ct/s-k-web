<script>
    import Icon from "@iconify/svelte";
    import { Link } from "svelte-routing";

    function showPurchaseDetails(){
        alert('aahh!.. my other!!')
    }

</script>

<main class="pt-4">
    <div class='bg-blue-500 flex text-white w-[150px] m-4 justify-center items-center'>
        <Icon icon='ic:outline-plus' />
        <p>New Purchase</p>
    </div>
    <div class="p-4 md:w-[80%] m-auto bg-white">
        <div class="flex justify-between">
            <div>
                show <input value="10" class="w-[40px] border-[1px] rounded-lg border-black mx-2" type="number" /> entries
            </div>
            <div>
                Search: <input class="border-[1px] border-black" type='text' />
            </div>
        </div>
        <div class="py-4">
            <table class="table-auto w-full border-collapse border border-slate-400 ">
                <thead>
                    <tr>
                        <th class="border border-slate-400 text-center">S/N</th>
                        <th class="border border-slate-400 text-center">Date</th>
                        <th class="border border-slate-400 text-center">Purchase Ref</th>
                        <th class="border border-slate-400 text-center">Item Purchased</th>
                        <th class="border border-slate-400 text-center">View More</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td class="border border-slate-300">1</td>
                        <td class="border border-slate-300">Dec 13, 2021</td>
                        <td class="border border-slate-300">#4059382</td>
                        <td class="border border-slate-300">Philip iron</td>
                        <td class="border border-slate-300 flex justify-center"> <button class="cursor-pointer" on:click={showPurchaseDetails}> <Icon icon='bi:eye-fill'/> </button>  </td>
                    </tr>
                </tbody>
            </table>
            <div class="flex justify-between items-center">
                <div>
                    Showing 1 to 5 of 5 items
                </div>
                <div class="flex items-center">
                    <button>
                        Next
                    </button>
                    <div class="p-2 mx-2 ">1</div>
                    <button>
                        prev
                    </button>
                </div>
            </div>
        </div>
    </div>
</main>