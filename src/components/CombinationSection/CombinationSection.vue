<template>
  <section class="combination-section">
    <icon />
    <heading>Combination Section</heading>
    <subtitle>
      It never was so easy to create a passive income in crypto.
    </subtitle>
    <advantages>
      <advantage-card
        v-for="(advantage, index) of advantages"
        :icon="advantage.icon"
        :title="advantage.title"
        :subtitle="advantage.subtitle"
        :key="index"
      />
    </advantages>
    <tile-button>Join</tile-button>
    <background-image :image="null" />
    <background-image :image="null" />
  </section>
</template>

<script>
import Icon from "./-Icon/Combination-Icon";
import Heading from "./-Heading/Combination-Heading";
import Subtitle from "./-Subtitle/CombinationSection-Subtitle";
import Advantages from "./-Advantages/CombinationSection-Advantages";
import AdvantageCard from "../AdvantageCard/AdvantageCard";
import TileButton from "../TileButton/TileButton";
import BackgroundImage from "./-BackgroundImage/CombinationSection-BackgroundImage";

export default {
  name: "CombinationSection",
  components: {
    Icon,
    Heading,
    Subtitle,
    Advantages,
    AdvantageCard,
    TileButton,
    BackgroundImage
  },
  data: () => ({
    advantages: [
      {
        icon: null,
        title: "Trade and mine at the same time",
        subtitle:
          "Receive rewards on your assets until the sell orders are confirmed"
      },
      {
        icon: null,
        title: "Mine BTC from your coins",
        subtitle:
          "Convert rewards to BTC immediately and earn BTC from your Proof-of-Stake coins using InstantSell"
      },
      {
        icon: null,
        title: "Maximise your profits",
        subtitle: "Reinvest coin rewards doubling the earnings in the long-term"
      },
      {
        icon: null,
        title: "Create your passive income portfolio with one click",
        subtitle:
          "Buy any coins on market price using InstantBuy or the exchange"
      }
    ]
  })
};
</script>

<style lang="stylus" scoped>
.combination-section
  display flex
  flex-direction column
  background rgba(9, 12, 19, 0.83)
</style>
