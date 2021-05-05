<script lang="ts">
	import Footer from "./Footer.svelte";
	import { GoogleAnalytics } from '@beyonk/svelte-google-analytics'
	import { Site } from "./types";
	import Header from "./Header.svelte";
	import SiteView from "./SiteView.svelte";
	const sites: Site[] = [
		{
			url: "https://rplanet.io/",
			title: "RPlanet Official Site",
			description: "Official website"
		},
		{
			url: "https://discord.gg/JNhHxkBwUB",
			title: "RPlanet Discord",
			description: "Official discord server"
		},
		{
			url: "https://link.medium.com/B60hrA4usfb",
			title: "Noob Guide",
			description: "Unofficial guide for new players"
		},
		{
			url: "https://t.me/rplanettrade",
			title: "Trading Telegram Chat",
			description: "Unofficial telegram chat for trading RPlanet NFTs"
		},
		{
			url: "https://rplanet.tools",
			title: "RPlanet Tools",
			description: "Features multiple tools like an automated elements generator and a staking calculator."
		},
		{
			url: "https://wax.simplemarket.io/trading/ft?&authors=a.rplanet&locale=en",
			title: "SimpleAssets Market",
			description: "Market for trading generated elements (Fungible Tokens or FTs)"
		},
		{
			url: "https://wax.alcor.exchange/trade/aether-e.rplanet_wax-eosio.token",
			title: "Alcor Exchange",
			description: "DEX for trading Aether and WAXP"
		},
		{
			url: "https://prospectors.online/alchemy/alchemy-recipes.html",
			title: "Successful Recipes",
			description: "List of updated successful recipes"
		},
		{
			url: "https://docs.google.com/spreadsheets/d/1Bu1ZE22ujitrkRoLBp_uptfezdQ9cVhUpDoukXb-NGM/edit#gid=588546488",
			title: "RPlanet Spreadsheet",
			description: "Community maintained spreadsheet that features staking values, recipes, and more"
		},
		{
			url: "http://rcalculator.net",
			title: "RCalculator",
			description: "Calculator for mining power that shows daily, weekly and monthly yield"
		},
		{
			url: "http://rplanet-staking-configs.vercel.app",
			title: "Staking Configs",
			description: "Staking configuration explorer that reads values from rplanets public contract"
		},
		{
			url: "https://rp.naw.io/",
			title: "Token Configurator",
			description: "Tool that adds RPlanets tokens configuration to your WAX Cloud Wallet"
		}

	];
</script>

<main>
	<GoogleAnalytics properties={["G-2FJZL5G2Q1"]} />
	<Header/>
	<div class="section">
			{#each sites as site}
				<SiteView {site} />
			{/each}
	</div>
	<Footer/>
</main>