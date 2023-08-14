<main class="pt-4">
    <div class="md:w-[80%] m-auto">
        <h2 class="p-4 bg-[#EEEEEE]">
            Inventory
        </h2>
        <div class="p-4 bg-white">
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
                            <th class="border border-slate-400 text-center">Product Name</th>
                            <th class="border border-slate-400 text-center">Stock In</th>
                            <th class="border border-slate-400 text-center">Stock Out</th>
                            <th class="border border-slate-400 text-center">stock Available</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td class="border border-slate-300">1</td>
                            <td class="border border-slate-300">Alcohol Name</td>
                            <td class="border border-slate-300">50</td>
                            <td class="border border-slate-300">16</td>
                            <td class="border border-slate-300">34</td>
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
    </div>
</main>