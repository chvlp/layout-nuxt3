<template>
    <v-navigation-drawer v-model="drawer">
        <img class="rounded-b-lg" src="/logo/pp.png" width="100%" alt="alt">
        <v-list nav>
            <v-list-subheader>Menu</v-list-subheader>

            <v-list>
                <v-list-item active-color="purple" v-for="([title, icon, to], i) in items" :key="i" :title="title"
                    :to="to" :prepend-icon="icon" :value="title" />
            </v-list>


            <v-list-group value="ຈັດການຂໍ້ມູນຜູ້ໃຊ້" active-color="purple">
                <template v-slot:activator="{ props }">
                    <v-list-item v-bind="props" prepend-icon="mdi-account" title="ຈັດການຂໍ້ມູນຜູ້ໃຊ້" />
                </template>

                <v-list-item active-color="purple" v-for="([title, icon, to], i) in items2" :key="i"
                    :prepend-icon="icon" :to="to" :title="title" :value="title" />
            </v-list-group>

        </v-list>

        <template v-slot:append>
            <div class="pa-2">
                <v-btn block>
                    Logout
                </v-btn>
            </div>
        </template>
    </v-navigation-drawer>


    <v-app-bar app elevation="0">

        <v-toolbar-title>{{ msg }} / <span class="text-caption">page</span> </v-toolbar-title>

        <v-spacer></v-spacer>

        <v-btn variant="text" icon="mdi-magnify"></v-btn>

        <v-btn variant="text" icon="mdi-filter"></v-btn>

        <v-btn variant="text" icon="mdi-dots-vertical"></v-btn>
        <v-app-bar-nav-icon variant="text" @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
    </v-app-bar>




</template>

<script>
export default {
    data: () => ({
        drawer: null,
        selectedItem: 1,
        items: [
            ['ໜ້າຫຼັກ', 'mdi-view-dashboard', '/'],
        ],
        items2: [
            ['ສິດທິຜູ້ໃຊ້', 'mdi-account-key', '/user/rule'],
            ['ຕຳເເໜ່ງຜູ້ໃຊ້', 'mdi-account-star', '/user/position'],
            ['ຜູູ້ໃຊ້', 'mdi-account-group', '/user'],
        ],
    }),
    props: { msg: String }

}
</script>

<style>
</style>