<template>
  <q-page class="flex">
      <div class="col">
        <div class="flex-break q-py-xl"></div>
        <div class="row justify-center">
            <q-input clearable rounded outlined class="col-8"
                placeholder="Search terms #tags">
                <template v-slot:append>
                    <q-avatar>
                        <q-icon name="search" />
                    </q-avatar>
                </template>
            </q-input>
        </div>
        <div class="flex-break q-py-md"></div>
        <div class="row justify-center">
            <q-list bordered separator>
                <q-item clickable v-ripple :active="active">
                    <q-item-section>
                        <q-input value="TJ's Pi"/>
                    </q-item-section>
                    <q-item-section>192.168.25.3</q-item-section>
                    <q-item-section side>Ubuntu</q-item-section>
                    <q-item-section side>22, 23, 80, 443</q-item-section>
                    <q-item-section avatar>
                        <q-icon color="positive" name="mdi-lan" />
                    </q-item-section>
                </q-item>
                <q-item clickable v-ripple :active="active">
                    <q-item-section>10.2.26.211</q-item-section>
                    <q-item-section side>Arch Linux</q-item-section>
                    <q-item-section side>22, 443</q-item-section>
                    <q-item-section avatar>
                        <q-icon color="negative" name="mdi-lan" />
                    </q-item-section>
                </q-item>
            </q-list>
        </div>
      </div>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex',
};
</script>
