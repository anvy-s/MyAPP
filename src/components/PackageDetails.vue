<script setup lang="ts">
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Basic</template>
    <a href="https://vuejs.org/" target="_blank" rel="noopener">AED 1200.99</a>
    <p>Set up a basic limited company and add anything else you need as extras.</p>
    <div style="padding-top: 50px;">
        <br/><br/><br/><br/><br/><br/><br/><br/><br/>
    <button class="button">Buy Now</button>
    </div>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Privacy</template>

    <a href="https://vitejs.dev/guide/features.html" target="_blank" rel="noopener">AED 1500.99</a>.
    <p>Your limited company formed with your home address protected from the public register.
        <br/>
        Includes Covent Garden registered office and service addresses.</p>
    <br/>
    More instructions are available in <code>README.md</code>.
    <div style="padding-top: 50px;">
        <br/>
        <br/>
        <br/>
        <br/>
    <button class="button">Buy Now</button>
    </div>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Compliance</template>

    <a href="https://vitejs.dev/guide/features.html" target="_blank" rel="noopener">AED 2500.99</a>.
        <p>A limited company formation package offering compliance and privacy.
        <br/>
        Includes filing of the first confirmation statement, GDPR pack, and VAT registration.
        <br/>
        Plus Covent Garden registered office and service address.
        <br/>
        Includes Covent Garden registered office and service addresses.</p>
    <br/>
    <div style="padding-top: 50px;">
    <button class="button">Buy Now</button>
    </div>

  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>All Inclusive</template>

    <a href="https://vitejs.dev/guide/features.html" target="_blank" rel="noopener">AED 3500.99</a>.
        <p>A limited company formation package offering compliance and privacy.
        <br/>
        Includes filing of the first confirmation statement, GDPR pack, and VAT registration.
        <br/>
        Plus Covent Garden registered office and service address.
        <br/>
        Includes Covent Garden registered office and service addresses.</p>
    <br/>
    <div style="padding-top: 50px;">
    <button class="button">Buy Now</button>
    </div>
  </WelcomeItem>

</template>

<style scoped>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}

.button {
  font-size: 18px;
  border-radius: 4px;
  background-color: #07a937;
  color: white;
  cursor: pointer;
  border: 2px solid #07a937;;
  height: 50px;
  width: 100px;
}
</style>