<template>
  <div>
    <section>
      <v-container>
        <v-row>
          <v-col>
            <h2>{{ appConfig.title }}</h2>
            <h3>Você é desenvolvedor? Cade sua página? Seus projetos?</h3>
            <hr />
            <headerDefault />
            <footerDefault />
            <br />
            <small>cores do sistema</small>
            <h6>{{ colors }}</h6>
          </v-col>
        </v-row>
      </v-container>
    </section>
    <section>
      <v-container>
        <v-row>
          <v-col cols="6">
            <p>oi mundo 1</p>
          </v-col>
          <v-col cols="6">
            <p>oi mundo 2</p>
          </v-col>
        </v-row>
      </v-container>
    </section>
  </div>
</template>

<script setup lang="ts">
const appConfig = useAppConfig();
const colors = appConfig.theme.colors;
</script>
