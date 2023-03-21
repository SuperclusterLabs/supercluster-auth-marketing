<script lang="ts">
	import Container from './Container.svelte';
	import manageImage from '$lib/assets/manage-image.png';
	import defineImage from '$lib/assets/define-image.png';
	import onboardImage from '$lib/assets/onboard-image.png';
</script>

<div class="relative mt-20 md:mt-40" id="features">
	<Container>
		<div class="mx-auto">
			<h3
				class="text-center text-2xl md:text-3xl text-black dark:text-white leading-loose md:leading-loose"
			>
				Supercluster Airlock is an <span class="font-bold text-planetYellow"
					>access management platform for your community</span
				>. It integrates web3 primitives with traditional web2 tooling into a simple platform where
				effective collaboration becomes a reality.
			</h3>
		</div>
		<div class="md:flex flex-row cols col-2 gap-6 mt-28">
			<div class="w-full md:w-1/2">
				<h3 class="mb-4 text-2xl md:text-3xl font-bold leading-relaxed">
					Easily manage your <span class="text-planetYellow">anonymous teams</span> and
					<span class="text-planetYellow">cohorts</span>
				</h3>
				<ul class="text-md mb-8 md:text-lg list-disc list-inside">
					<li>Define your access requirements using web3 and web2 engagement primitives.</li>
					<li>Your community members will automatically get access to your tools.</li>
					<li>No more doxxing.</li>
				</ul>
			</div>
			<div>
				<img src={manageImage} alt="Manage anonymous teams and cohorts" />
			</div>
		</div>
		<div class="md:flex flex-row cols col-2 gap-6 mt-28">
			<div class="w-full md:w-1/2">
				<h3 class="mb-4 text-2xl md:text-3xl font-bold leading-relaxed">
					<span class="text-planetYellow">Define</span> and
					<span class="text-planetYellow">automate</span> your community’s access requirements
				</h3>
				<ul class="mb-8 text-md md:text-lg list-disc list-inside">
					<li>
						Once your access requirements are defined, access is automatically enforced by Airlock.
					</li>
					<li>
						As users engage more, they will automatically gain access to additional tooling, defined
						by your team.
					</li>
				</ul>
			</div>
			<div class="sm:flex-2">
				<img class="w-[450px]" src={defineImage} alt="Manage anonymous teams and cohorts" />
			</div>
		</div>
		<div class="md:flex flex-row cols col-2 gap-6 mt-28">
			<div class="w-full md:w-1/2">
				<h3 class="mb-4 text-2xl md:text-3xl font-bold leading-relaxed">
					<span class="text-planetYellow">Onboard</span> your new contributors to all your tools, at
					once.
				</h3>
				<ul class="mb-8 text-md md:text-lg list-disc list-inside">
					<li>Integrate all the tools that your community or team uses.</li>
					<li>
						When a new contributor joins, they’ll be able to easily see and access all the tools
						they need to get started.
					</li>
				</ul>
			</div>
			<div>
				<img class="w-[650px]" src={onboardImage} alt="Manage anonymous teams and cohorts" />
			</div>
		</div>
	</Container>
</div>
