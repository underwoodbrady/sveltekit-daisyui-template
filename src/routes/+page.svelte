<script lang="ts">
	import One from 'virtual:icons/material-symbols/imagesmode-rounded';
	import Night from 'virtual:icons/material-symbols/bedtime';
	import Day from 'virtual:icons/material-symbols/sunny-rounded';
</script>

<div class="navbar bg-base-300 rounded-box">
	<div class="flex-1 px-2 lg:flex-none">
		<a class="text-lg font-bold">daisyUI</a>
	</div>
	<div class="flex justify-end flex-1 px-2">
		<div class="flex items-stretch">
			<a class="btn btn-ghost rounded-btn">Button</a>
			<div class="dropdown dropdown-end">
				<div tabindex="0" role="button" class="btn btn-ghost rounded-btn">Dropdown</div>
				<ul
					tabindex="0"
					class="menu dropdown-content z-[1] p-2 shadow bg-base-100 rounded-box w-52 mt-4"
				>
					<li><a>Item 1</a></li>
					<li><a>Item 2</a></li>
				</ul>
			</div>
			<button class="btn" onclick="my_modal_3.showModal()">open modal</button>
		</div>
	</div>
</div>

<header>
	<h2 class="font-semibold text-xl">Welcome to SvelteKit</h2>
	<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
	<label class="flex cursor-pointer gap-2">
		<Night />
		<input type="checkbox" value="light" class="toggle theme-controller" />
		<Day />
	</label>
</header>

<section>
	<div class="card bg-base-300 shadow-xl">
		<div class="card-body">
			<h2 class="card-title">Buttons</h2>
			<button class="btn btn-primary">Button</button>
			<button class="btn btn-neutral">Neutral</button>
			<button class="btn btn-link">Link</button>
			<button class="btn btn-square">
				<span class="loading loading-spinner"></span>
			</button>
			<button class="btn">
				Button
				<One class="text-lg text-primary" />
			</button>
		</div>
	</div>
	<div class="card bg-base-300 shadow-xl">
		<div class="card-body">
			<h2 class="card-title">Dropdowns</h2>
			<div class="dropdown">
				<div tabindex="0" role="button" class="btn m-1">Click</div>
				<!-- svelte-ignore a11y-no-noninteractive-tabindex -->
				<ul
					tabindex="0"
					class="dropdown-content z-[1] menu p-2 shadow bg-base-100 rounded-box w-52"
				>
					<!-- svelte-ignore a11y-missing-attribute -->
					<li><a>Item 1</a></li>
					<!-- svelte-ignore a11y-missing-attribute -->
					<li><a>Item 2</a></li>
				</ul>
			</div>
		</div>
	</div>
	<div class="card bg-base-300 shadow-xl">
		<div class="card-body">
			<h2 class="card-title">Badges</h2>
			<div class="badge">default</div>
			<div class="badge badge-neutral">neutral</div>
			<div class="badge badge-primary">primary</div>
		</div>
	</div>
    <div>
        <div class="stats shadow">
  
            <div class="stat">
              <div class="stat-figure text-primary">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" class="inline-block w-8 h-8 stroke-current"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"></path></svg>
              </div>
              <div class="stat-title">Total Likes</div>
              <div class="stat-value text-primary">25.6K</div>
              <div class="stat-desc">21% more than last month</div>
            </div>
            
            <div class="stat">
              <div class="stat-figure text-secondary">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" class="inline-block w-8 h-8 stroke-current"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path></svg>
              </div>
              <div class="stat-title">Page Views</div>
              <div class="stat-value text-secondary">2.6M</div>
              <div class="stat-desc">21% more than last month</div>
            </div>
            
            <div class="stat">
              <div class="stat-figure text-secondary">
                <div class="avatar online">
                  <div class="w-16 rounded-full">
                    <img src="https://daisyui.com/images/stock/photo-1534528741775-53994a69daeb.jpg" />
                  </div>
                </div>
              </div>
              <div class="stat-value">86%</div>
              <div class="stat-title">Tasks done</div>
              <div class="stat-desc text-secondary">31 tasks remaining</div>
            </div>
            
          </div>
    </div>
</section>



<dialog id="my_modal_3" class="modal">
	<div class="modal-box">
		<form method="dialog">
			<button class="btn btn-sm btn-circle btn-ghost absolute right-2 top-2">✕</button>
		</form>
		<h3 class="font-bold text-lg">Hello!</h3>
		<p class="py-4">Press ESC key or click on ✕ button to close</p>
	</div>
</dialog>
