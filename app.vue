<template>
  <Html>
    <Head>
    </Head>
    <Body>
      <div>
        <div>
          <NuxtLayout>
            <div>
              <NuxtPage />
            </div>
          </NuxtLayout>
        </div>
      </div>
    </Body>
  </Html>
</template>

<script setup>

const initMetrika = () => {
    // Metrika

    (function(m,e,t,r,i,k,a){m[i]=m[i]||function(){(m[i].a=m[i].a||[]).push(arguments)};
      m[i].l=1*new Date();
      for (var j = 0; j < document.scripts.length; j++) {if (document.scripts[j].src === r) { return; }}
      k=e.createElement(t),a=e.getElementsByTagName(t)[0],k.async=1,k.src=r,a.parentNode.insertBefore(k,a)})
    (window, document, "script", "https://mc.yandex.ru/metrika/tag.js", "ym");

    window.ym(95986825, "init", {
        clickmap:true,
        trackLinks:true,
        accurateTrackBounce:true,
        webvisor:true
    })
}

onMounted(async () => {
  initMetrika()
})

</script>
