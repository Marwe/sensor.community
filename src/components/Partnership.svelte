<script>
    import initI18n from "../utils/initI18n";
    import {stores} from "@sapper/app";

    const {page} = stores();
    $: lang = $page.params.lang;
    $: i18n = initI18n(lang);
</script>

<section class="py-4 md:py-10">
    <div class="container mx-auto pt-10 md:pt-0 flex flex-col">

        <h2 class="w-full py-4 md:py-8 text-gray-700 text-5xl md:text-5xl font-bold leading-normal text-center">
            {i18n.t('partnership:title')}</h2>

        <div class="flex flex-wrap justify-center md:justify-between items-center mt-6 opacity-75 mx-auto">
            <a href="https://www.opengeospatial.org/" target="_blank"
               class="w-1/5 px-2 mb-4 md:mb-2 md:px-2 md:w-auto inline-block text-center">
                <img src="images/partner/ogc.png"></a>
            <a href="https://www.rivm.nl/" target="_blank"  class="w-1/5 px-2 mb-4 md:mb-2 md:px-2 md:w-auto inline-block text-center">
                <img src="images/partner/rivm.png"></a>
            <a href="https://www.opengeospatial.org/" target="_blank"
               class="w-1/5 px-2 mb-4 md:mb-2 md:px-2 md:w-auto inline-block text-center">
                <img src="images/partner/jrc.png"></a>
        </div>
    </div>
</section>
