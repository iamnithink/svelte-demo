<script lang="ts">
  import { Router, Route} from 'svelte-navigator';
  import Articles from './pages/Articles.svelte';
  import InvestingAdvice from './pages/InvestingAdvice.svelte';
  import MyFavoriteFrontendFramework from './pages/MyFavoriteFrontendFramework.svelte';
  import ReactvsSvelte from './pages/ReactvsSvelte.svelte';
  import VueVsAngular from './pages/VueVsAngular.svelte';
</script>

<Router>
  <Route path="/">
    <Articles />
  </Route>
  <Route path="/react-vs-svelte">
    <ReactvsSvelte />
  </Route>
  <Route path="/investing-advice">
    <InvestingAdvice />
  </Route>
  <Route path="/my-favorite-frontend-framework">
    <MyFavoriteFrontendFramework />
  </Route>
  <Route path="/vue-vs-angular">
    <VueVsAngular />
  </Route>
</Router>

<style global lang="postcss">
@tailwind base;
@tailwind components;
@tailwind utilities;
</style>