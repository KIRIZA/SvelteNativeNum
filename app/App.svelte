<page actionBarHidden={true}>
   <tabs bind:selectedIndex={selectedTab} tabsPosition='bottom'>
	<tabStrip class='blue'>
		<tabStripItem>
			<label text="Page 1" />
		</tabStripItem>
		</tabStrip>

	<tabContentItem>
        <cardView margin='32' elevation='40'>
            <Page1 />
        </cardView>
	</tabContentItem>       
</tabs>
</page>

<script>
//first: tns plugin add @nstudio/nativescript-cardview
import { registerNativeViewElement } from 'svelte-native/dom' 
registerNativeViewElement("cardView", () => 
    require("@nstudio/nativescript-cardview").CardView
)
    import Page1 from './screens/Page1.svelte'
    
    let selectedTab = 0
</script>

<style>
    .blue{
        padding:24;
        }
    
</style>