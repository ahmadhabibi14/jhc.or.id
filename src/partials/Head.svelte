<script lang="ts">
	import { SiteName, SiteDesc, SiteBaseUrl, SiteImageUrl, SiteAuthor } from '../lib/constant';

	export let title: string = SiteName;
	export let path: string = '';
	export let description: string = SiteDesc;
	export let imageUrl: string = SiteImageUrl;
	export let author: string = SiteAuthor;
	export let imgWidth: string = '1200';
	export let imgHeight: string = '630';

	const siteUrl: string = SiteBaseUrl + path;
</script>

<svelte:head>
	<title>{title}</title>
	<meta http-equiv="x-ua-compatible" content="ie=edge" />
	<meta name="author" content={author} />
	<meta name="description" content={description} />
	<meta name="referrer" content="no-referrer-when-downgrade" />

	<meta property="og:site_name" content={title} />
	<meta property="og:title" content={title} />
	<meta property="og:description" content={description} />
	<meta property="og:locale" content="id_ID" />
	<meta property="og:locale:alternate" content="en_UK" />
	<meta property="og:locale:alternate" content="ms_MY" />
	<meta property="og:type" content="website" />
	<meta property="og:url" content={siteUrl} />
	<meta property="og:image" content={imageUrl ? imageUrl : SiteImageUrl} />
	<meta property="og:image:secure_url" content={imageUrl ? imageUrl : SiteImageUrl} />
	<meta property="og:image:width" content={imgWidth} />
	<meta property="og:image:height" content={imgHeight} />
	<meta property="og:image:alt" content={title} />
	<meta property="og:see_also" content="https://www.instagram.com/jayakartahalalcenter/" />

	<meta name="twitter:card" content="summary_large_image" />
	<meta name="twitter:title" content={title} />
	<meta name="twitter:description" content={description} />
	<meta name="twitter:image" content={imageUrl} />
	<meta name="twitter:image:width" content={imgWidth} />
	<meta name="twitter:image:height" content={imgHeight} />

	<meta name="DC.title" content="Geo Tag Generator" />
	<meta name="geo.region" content="ID-JK" />
	<meta name="geo.placename" content="Jakarta Timur, DKI Jakarta" />
	<meta name="geo.position" content="-6.333851, 106.902487" />
	<meta name="ICBM" content="-6.333851, 106.902487" />

	<link href={SiteBaseUrl} rel="canonical" />
	<link href={SiteBaseUrl} rel="home" />
	<link type="text/plain" href="{SiteBaseUrl}/humans.txt" rel="author" />

	<script type="application/ld+json">
		{
			"@context": "https://schema.org",
			"@graph": [
				{
					"@type": ["Person", "Organization"],
					"@id": "https://jhc.or.id/#person",
					"name": "Prima Halal Cendekia",
					"logo": {
						"@type": "ImageObject",
						"@id": "https://jhc.or.id/#logo",
						"url": "https://jhc.or.id/wp-content/uploads/2026/01/logo-prima-halal-cendekia-removebg-preview.png",
						"contentUrl": "https://jhc.or.id/wp-content/uploads/2026/01/logo-prima-halal-cendekia-removebg-preview.png",
						"caption": "Prima Halal Cendekia",
						"inLanguage": "en-US",
						"width": "1046",
						"height": "238"
					},
					"image": {
						"@type": "ImageObject",
						"@id": "https://jhc.or.id/#logo",
						"url": "https://jhc.or.id/wp-content/uploads/2026/01/logo-prima-halal-cendekia-removebg-preview.png",
						"contentUrl": "https://jhc.or.id/wp-content/uploads/2026/01/logo-prima-halal-cendekia-removebg-preview.png",
						"caption": "Prima Halal Cendekia",
						"inLanguage": "en-US",
						"width": "1046",
						"height": "238"
					}
				},
				{
					"@type": "WebSite",
					"@id": "https://jhc.or.id/#website",
					"url": "https://jhc.or.id",
					"name": "Prima Halal Cendekia",
					"alternateName": "Prima Halal Cendekia",
					"publisher": { "@id": "https://jhc.or.id/#person" },
					"inLanguage": "en-US",
					"potentialAction": {
						"@type": "SearchAction",
						"target": "https://jhc.or.id/?s={search_term_string}",
						"query-input": "required name=search_term_string"
					}
				},
				{
					"@type": "ImageObject",
					"@id": "https://jhc.or.id/wp-content/uploads/2026/02/Sertifikasi-Halal-MBG-SPPG-Prima-Halal-Cendekia-1024x576.webp",
					"url": "https://jhc.or.id/wp-content/uploads/2026/02/Sertifikasi-Halal-MBG-SPPG-Prima-Halal-Cendekia-1024x576.webp",
					"width": "200",
					"height": "200",
					"inLanguage": "en-US"
				},
				{
					"@type": "WebPage",
					"@id": "https://jhc.or.id/#webpage",
					"url": "https://jhc.or.id/",
					"name": "Jasa Sertifikasi Halal Resmi &amp; Terpercaya - Prima Halal Cendekia",
					"datePublished": "2026-01-20T18:18:37-07:00",
					"dateModified": "2026-02-01T07:06:16-07:00",
					"about": { "@id": "https://jhc.or.id/#person" },
					"isPartOf": { "@id": "https://jhc.or.id/#website" },
					"primaryImageOfPage": {
						"@id": "https://jhc.or.id/wp-content/uploads/2026/02/Sertifikasi-Halal-MBG-SPPG-Prima-Halal-Cendekia-1024x576.webp"
					},
					"inLanguage": "en-US"
				},
				{
					"@type": "Person",
					"@id": "https://jhc.or.id/#author",
					"name": "admin",
					"image": {
						"@type": "ImageObject",
						"@id": "https://secure.gravatar.com/avatar/5a722d9d524897978c0607ccefcc5c46fb84f7daa7db7c9d1f5e0c856ae96cd4?s=96&amp;d=mm&amp;r=g",
						"url": "https://secure.gravatar.com/avatar/5a722d9d524897978c0607ccefcc5c46fb84f7daa7db7c9d1f5e0c856ae96cd4?s=96&amp;d=mm&amp;r=g",
						"caption": "admin",
						"inLanguage": "en-US"
					},
					"sameAs": ["https://jhc.or.id"]
				},
				{
					"@type": "Article",
					"headline": "Jasa Sertifikasi Halal Resmi &amp; Terpercaya - Prima Halal Cendekia",
					"keywords": "Jasa Sertifikasi Halal,Buat Sertifikat Halal,Konsultan Halal,Sertifikasi Halal UMKM,Sertifikasi Halal Restoran,Sertifikasi Halal Katering,Penyelia Halal,Prima Halal Cendekia",
					"datePublished": "2026-01-20T18:18:37-07:00",
					"dateModified": "2026-02-01T07:06:16-07:00",
					"author": { "@id": "https://jhc.or.id/#author", "name": "admin" },
					"publisher": { "@id": "https://jhc.or.id/#person" },
					"description": "Konsultan Jasa Sertifikasi Halal resmi BPJPH &amp; MUI. Layanan cepat &amp; full pendampingan untuk UMKM, Katering, Restoran, Industri, dan Dapur MBG. Jaminan terbit sertifikat.",
					"name": "Jasa Sertifikasi Halal Resmi &amp; Terpercaya - Prima Halal Cendekia",
					"@id": "https://jhc.or.id/#richSnippet",
					"isPartOf": { "@id": "https://jhc.or.id/#webpage" },
					"image": {
						"@id": "https://jhc.or.id/wp-content/uploads/2026/02/Sertifikasi-Halal-MBG-SPPG-Prima-Halal-Cendekia-1024x576.webp"
					},
					"inLanguage": "en-US",
					"mainEntityOfPage": { "@id": "https://jhc.or.id/#webpage" }
				}
			]
		}
	</script>
</svelte:head>
