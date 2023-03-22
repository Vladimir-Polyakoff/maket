<script>
import Menu from '@/components/Menu'
import Header from '@/components/Header'
import DiscoverCard from '@/components/DiscoverCard'
import MonthlyDeals from '@/components/MonthlyDeals'
import RecentNews from '@/components/RecentNews'
import Bestseller from '@/components/Bestseller'
import Testimonials from '@/components/Testimonials'
import Instagram from '@/components/Instagram'
import Sponsor from '@/components/Sponsor'

export default {
  name: 'TheHeader',

  components: {
    Menu,
    Header,
    DiscoverCard,
    MonthlyDeals,
    RecentNews,
    Bestseller,
    Testimonials,
    Instagram,
    Sponsor
  }
}
</script>

<template>
  <div>
    <Menu></Menu>
    <Header></Header>
    <DiscoverCard></DiscoverCard>
    <MonthlyDeals></MonthlyDeals>
    <RecentNews></RecentNews>
    <Bestseller></Bestseller>
    <Testimonials></Testimonials>
    <Instagram></Instagram>
    <Sponsor></Sponsor>
  </div>
</template>

<style scoped>
</style>
