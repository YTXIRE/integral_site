<template>
    <div>
        <AboutUs/>
        <Sand/>
        <Macadam/>
        <Armature/>
        <WhatWeDo/>
        <Contacts/>
    </div>
</template>

<script>
import AboutUs from "./AboutUs";
import Sand from "./Sand";
import Macadam from "./Macadam";
import Armature from "./Armature";
import WhatWeDo from "./WhatWeDo";
import Contacts from "./Contacts";

export default {
    name: "Main",
    components: {WhatWeDo, Sand, AboutUs, Macadam, Armature, Contacts}
}
</script>