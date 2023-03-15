<script setup lang="ts">
/**
 * This is a Vue Component that will be
 * automatically mapped to a entry on vue-router.
 *
 * You will be able to access this page at http://localhost:3000/starters/sideblock-blank-page-1
 * Page uri will match related path to src/pages folder
 *
 * Read more about routing:
 * @see /vite.config.ts
 * @see /src/router.ts
 */

import { useHead } from '@vueuse/head'
import { useViewWrapper } from '/@src/stores/viewWrapper'

const viewWrapper = useViewWrapper()
viewWrapper.setPageTitle('北京某某科技公司')

useHead({
  title: '北京某某科技公司',
})
</script>

<template>
  <IndexLayout theme="float" open-on-mounted>
    <!-- Content Wrapper -->
    <div class="page-content-inner">

      <BankingDashboardV1></BankingDashboardV1>
    </div>
  </IndexLayout>
</template>
