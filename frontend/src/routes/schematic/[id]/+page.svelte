<script lang="ts">
  import Slider from "$lib/Slider.svelte";

  const tags = ["farm", "Above & Beyond"];
  const mods = ["Create: Steam 'n' Rails", "Create: Extended Bogeys", "aa", "bb", "cc"];
</script>

<main
  class="max-w-6xl w-[calc(100vw-2rem)] flex flex-col mx-auto gap-3"
>
  <section class="flex gap-3 w-full justify-stretch flex-wrap md:flex-nowrap">
    <div class="flex md:w-2/3 aspect-video bg-minecraft-ui-dark p-3 pixel-corners">
      <Slider
        images={[
          "https://picsum.photos/800/450",
          "https://picsum.photos/800/450",
          "https://picsum.photos/800/450",
        ]}
      />
    </div>
    <div class="flex flex-col gap-2 w-full md:w-1/3 justify-between bg-minecraft-ui-dark pixel-corners">
      <div class="flex flex-col gap-2">
        <div class="p-3 pb-0">
          <h1 class="text-2xl font-bold">Very cool schematic</h1>
          <h3 class="text-xs text-white/50">
            by <a href="/user/Szedann" class="underline">Szedann</a>
          </h3>
        </div>
        <div class="px-2 text-sm pixel-corners p-2 flex bg-black m-2 divide-x divide-create-blue/20">
          <div class="flex flex-col items-center w-full">
            <h1 class="text-xl">603</h1>
            <span class="text-xs">Donwloads</span>
          </div>
          <div class="flex flex-col items-center w-full">
            <h1 class="text-xl">60%</h1>
            <span class="text-xs">Likes</span>
          </div>
          <div class="flex flex-col items-center w-full">
            <h1 class="text-xl">894</h1>
            <span class="text-xs">Views</span>
          </div>
        </div>
        <ul class="flex flex-wrap gap-2 px-2">
          {#each tags as tag}
            <li
              class="text-xs bg-create-blue/20 px-1 text-white/50">
              {tag}
            </li>
          {/each}
        </ul>
        <div class="w-full p-3 bg-checker bg-black/20">
          <h2>Required mods:</h2>
          <ul class="flex flex-col gap-2 overflow-y-scroll max-h-64 p-2 bg-fixed no-scrollbar">
            {#each mods as mod}
              <li
                class="flex gap-2 bg-black/30 w-full p-2 pixel-corners bg-checker">
                <img src="https://picsum.photos/40" alt="" class="pixel-corners aspect-square" />
                <div>
                  <h2 class="font-bold">{mod}</h2>
                  <div class="text-xs flex gap-1 font-mono">
                    <a href="https://modrinth.com">Modrinth</a>
                    <a href="https://cursefurge.com">CurseForge</a>
                  </div>
                </div>
              </li>
            {/each}
          </ul>
        </div>
      </div>
      <div class="flex flex-col gap-3 p-3 pt-0">
        <a
          href="create-schem://123124"
          style="--checker-color: #0001"
          class="w-full bg-green-500 text-xl p-2 text-center font-bold pixel-corners bg-checker"
          >Download</a
        >
      </div>
    </div>
  </section>
  <section class="bg-minecraft-ui-dark p-3 pixel-corners">
    <nav class="my-3 flex gap-2">
      <h2 class="text-xl underline">Description</h2>
      <h2 class="text-xl text-white/50">Details</h2>
  
    </nav>
    <div class="bg-black/50 p-4 pixel-corners">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem
      blanditiis dolores quaerat iste veritatis. Sequi saepe, ut aut voluptatem
      enim rerum! Debitis praesentium error aliquam. Deserunt doloremque numquam
      eligendi alias sit explicabo. Laboriosam cum dolor eaque voluptas id
      quisquam optio iste maxime, totam dicta libero reprehenderit facilis eum
      quaerat magni aliquam, commodi, nam corporis. Ratione impedit repellat
      temporibus maiores ad? Quis quam necessitatibus, tempora incidunt fugiat
      perspiciatis quibusdam ipsam suscipit recusandae veniam modi quaerat,
      debitis, qui dolorum! Deleniti nihil non ut molestiae facere maxime
      officia error praesentium, eveniet doloribus, impedit blanditiis autem
      amet voluptatibus atque dolor enim? Animi ullam minus aliquam quaerat
      adipisci earum maxime magnam odio ducimus illum soluta iure dolores
      asperiores consequuntur numquam consectetur incidunt, impedit ex officia
      aut deleniti vitae dolore neque doloremque. Odio architecto vitae, iure,
      aliquam quia expedita consequuntur quam accusamus magnam ipsum
      repellendus. Beatae facilis iste, odit repellendus voluptates nemo dolorum
      error. Sed praesentium quo eos, saepe voluptatibus doloremque repellendus
      asperiores odit vel maiores. Reiciendis autem amet earum, nostrum eius
      suscipit, deserunt voluptatum nisi unde dignissimos maxime eum similique
      sunt repellendus voluptatibus quasi culpa commodi quibusdam veniam, animi
      cum. Quos sit aperiam, expedita consequuntur, tenetur nostrum dolorem
      nihil commodi ipsa officiis quasi obcaecati! In.
    </div>
  </section>
</main>
