<script lang="ts">
	import FeatureBlock from './FeatureBlock.svelte';
</script>

<!-- Block 1: Complete API Coverage -->
<FeatureBlock 
	title="200+ endpoints with complete coverage" 
	description="Full OnlyFans API access including login system with 2FA, face verification, messages, subscriptions, and revenue tracking."
	buttons={[
		{ text: "VIEW DOCUMENTATION", icon: true },
		{ text: "TRY PLAYGROUND" }
	]}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm p-4 font-mono text-xs">
		<div class="flex items-center gap-2 border-b border-border pb-2 mb-4">
			<span class="text-primary-600">GET</span>
			<span class="text-muted">/api/v1/messages</span>
			<span class="ml-auto text-green-600 text-[10px]">200 OK</span>
		</div>
		<div class="space-y-3 text-[10px]">
			<div class="flex items-center gap-2">
				<div class="w-1 h-1 bg-primary-600 rounded-full"></div>
				<span class="text-gray-600">Authentication & 2FA</span>
			</div>
			<div class="flex items-center gap-2">
				<div class="w-1 h-1 bg-primary-600 rounded-full"></div>
				<span class="text-gray-600">Messages & Chat</span>
			</div>
			<div class="flex items-center gap-2">
				<div class="w-1 h-1 bg-primary-600 rounded-full"></div>
				<span class="text-gray-600">Subscriptions & Revenue</span>
			</div>
			<div class="flex items-center gap-2">
				<div class="w-1 h-1 bg-primary-600 rounded-full"></div>
				<span class="text-gray-600">Posts & Media</span>
			</div>
		</div>
	</div>
</FeatureBlock>

<!-- Block 2: Zero-Ban Security -->
<FeatureBlock 
	title="Zero-ban security infrastructure" 
	description="5+ years of operation with zero account bans. AES-256 encryption, isolated systems, and dedicated proxy infrastructure."
	buttons={[
		{ text: "SECURITY DETAILS", icon: true }
	]}
	alignRight={true}
>
	<div class="w-full max-w-md bg-gradient-to-br from-gray-900 to-black border border-gray-700 rounded shadow-sm p-6 flex flex-col gap-4">
		<div class="flex items-center gap-2 text-xs font-mono text-green-400">
			<svg width="16" height="16" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
				<path d="M12 2L4 6v6c0 5.55 3.84 10.74 8 12 4.16-1.26 8-6.45 8-12V6l-8-4z" stroke="currentColor" stroke-width="2"/>
				<path d="M9 12l2 2 4-4" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
			</svg>
			Security Status: Active
		</div>
		<div class="space-y-3">
			<div class="flex justify-between items-center text-[10px] text-gray-400">
				<span>Accounts Protected</span>
				<span class="text-white font-semibold">10,000+</span>
			</div>
			<div class="flex justify-between items-center text-[10px] text-gray-400">
				<span>Years Operating</span>
				<span class="text-white font-semibold">5+</span>
			</div>
			<div class="flex justify-between items-center text-[10px] text-gray-400">
				<span>Account Bans</span>
				<span class="text-green-400 font-semibold">0</span>
			</div>
		</div>
		<div class="mt-2 pt-3 border-t border-gray-700 flex items-center gap-2 text-[10px] text-gray-400 font-mono">
			<span class="w-2 h-2 bg-green-500 rounded-full animate-pulse"></span>
			AES-256 ENCRYPTED
		</div>
	</div>
</FeatureBlock>

<!-- Block 3: Real-time Webhooks -->
<FeatureBlock 
	title="Real-time webhooks & automation" 
	description="HMAC-signed webhooks for messages, sales, renewals, and subscribers. Automate your entire creator workflow."
	buttons={[
		{ text: "WEBHOOK DOCS", icon: true }
	]}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm overflow-hidden font-mono text-[10px]">
		<div class="grid grid-cols-4 gap-2 p-2 border-b border-border bg-gray-50 text-muted">
			<div>EVENT</div>
			<div>STATUS</div>
			<div>TIME</div>
			<div>ACTION</div>
		</div>
		{#each [
			{ event: 'message.new', status: 'delivered', color: 'green' },
			{ event: 'subscription.new', status: 'delivered', color: 'green' },
			{ event: 'payment.received', status: 'delivered', color: 'green' },
			{ event: 'renewal.success', status: 'delivered', color: 'green' },
			{ event: 'message.new', status: 'delivered', color: 'green' },
			{ event: 'tip.received', status: 'delivered', color: 'green' }
		] as item, i}
			<div class="grid grid-cols-4 gap-2 p-2 border-b border-border/50 items-center">
				<div class="flex items-center gap-1">
					<div class="w-1.5 h-1.5 rounded-full bg-primary-500"></div>
					<span class="text-gray-700">{item.event}</span>
				</div>
				<div class="flex items-center gap-1">
					<span class="text-{item.color}-600">✓ {item.status}</span>
				</div>
				<div class="text-muted">{i}ms</div>
				<div class="h-1.5 w-12 bg-gray-100 rounded"></div>
			</div>
		{/each}
	</div>
</FeatureBlock>

<!-- Block 4: Developer Dashboard -->
<FeatureBlock 
	title="Live API playground & dashboard" 
	description="Test endpoints in your browser, monitor usage, manage API keys, and view real-time logs. Complete developer experience."
	buttons={[
		{ text: "TRY PLAYGROUND", icon: true }
	]}
	alignRight={true}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm overflow-hidden">
		<div class="border-b border-border bg-gray-50 p-2 flex items-center gap-2 text-[10px] font-mono">
			<div class="flex items-center gap-1">
				<div class="w-2 h-2 rounded-full bg-red-500"></div>
				<div class="w-2 h-2 rounded-full bg-yellow-500"></div>
				<div class="w-2 h-2 rounded-full bg-green-500"></div>
			</div>
			<span class="text-muted">API Playground</span>
		</div>
		<div class="p-4 font-mono text-[10px] space-y-3">
			<div class="flex items-center gap-2">
				<span class="text-primary-600 font-semibold">POST</span>
				<span class="text-gray-600">/api/v1/messages/send</span>
			</div>
			<div class="bg-gray-50 p-2 rounded border border-gray-200">
				<div class="text-gray-500">{"{"}</div>
				<div class="pl-3 text-gray-700">"text": "Hello from API",</div>
				<div class="pl-3 text-gray-700">"userId": "12345"</div>
				<div class="text-gray-500">{"}"}</div>
			</div>
			<button class="w-full bg-primary-600 text-white py-2 rounded text-xs font-semibold hover:bg-primary-700 transition-colors">
				Send Request
			</button>
			<div class="bg-green-50 border border-green-200 p-2 rounded">
				<div class="text-green-700 font-semibold mb-1">✓ 200 OK</div>
				<div class="text-green-600 text-[9px]">Response time: 287ms</div>
			</div>
		</div>
	</div>
</FeatureBlock>

<!-- Block 5: Enterprise Support -->
<FeatureBlock 
	title="White glove enterprise support" 
	description="Dedicated support channels, custom development services, and fast response times. Build bespoke solutions with our team."
	buttons={[
		{ text: "BOOK A CALL", icon: true }
	]}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm p-4 flex flex-col gap-4">
		<div class="flex items-center justify-between border-b border-border pb-3">
			<div class="text-xs font-semibold">Support Channels</div>
			<div class="flex items-center gap-1 text-[10px] text-green-600 font-mono">
				<span class="w-2 h-2 bg-green-500 rounded-full"></span>
				Online
			</div>
		</div>
		
		<div class="space-y-3">
			<div class="flex items-center gap-3 p-2 bg-gray-50 rounded border border-gray-200">
				<div class="w-8 h-8 bg-blue-500 rounded flex items-center justify-center text-white text-xs font-bold">
					T
				</div>
				<div class="flex-1">
					<div class="text-xs font-semibold">Telegram</div>
					<div class="text-[10px] text-muted">Instant messaging</div>
				</div>
			</div>

			<div class="flex items-center gap-3 p-2 bg-gray-50 rounded border border-gray-200">
				<div class="w-8 h-8 bg-green-500 rounded flex items-center justify-center text-white text-xs font-bold">
					W
				</div>
				<div class="flex-1">
					<div class="text-xs font-semibold">WhatsApp</div>
					<div class="text-[10px] text-muted">Direct support</div>
				</div>
			</div>

			<div class="flex items-center gap-3 p-2 bg-gray-50 rounded border border-gray-200">
				<div class="w-8 h-8 bg-gray-700 rounded flex items-center justify-center text-white text-xs font-bold">
					@
				</div>
				<div class="flex-1">
					<div class="text-xs font-semibold">Email</div>
					<div class="text-[10px] text-muted">Detailed inquiries</div>
				</div>
			</div>
		</div>

		<div class="mt-auto pt-3 border-t border-border">
			<div class="text-[10px] text-muted font-mono">
				Average response time: <span class="text-foreground font-semibold">&lt; 2 hours</span>
			</div>
		</div>
	</div>
</FeatureBlock>
