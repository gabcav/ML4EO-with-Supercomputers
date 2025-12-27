# Background and Context 

Remote Sensing (RS) has come a long way since 1858, when Gaspard-Félix Tournachon, known by the pseudonym Nadar, captured the first aerial photograph from a hot air balloon over the Paris suburb of [Petit-Bicêtre](https://blog.historicaerials.com/nadar-and-the-first-aerial-photograph/). The ability to photograph the Earth from above has had a massive cultural influence. In the nineteenth century, Nadar’s hot-air balloon photography inspired author [Jules Verne](https://fai.org/sites/default/files/documents/cia-hof-tournachon-gaspar.pdf). In the twentieth, the [Blue Marble](https://en.wikipedia.org/wiki/The_Blue_Marble) (an image of Earth taken during the Apollo 17 mission) inspired a generation of [environmental activists](https://static1.squarespace.com/static/550c93a2e4b0567de63a74a4/t/58b4b63c5016e12e671cf026/1488238141010/Essay_Wolthers.pdf). While Landsat launched in 1972, the "big data" era was truly kickstarted by the 2008 open data policy, which made the archive available at no cost and [unlocked its true value](https://www.usgs.gov/centers/eros/news/opening-landsat-archive-helped-realize-its-true-value). The development of artificial satellites in the latter half of the 20th century allowed Earth Observation (EO) to progress to a global scale.

Enormous investments in satellite constellations like [MODIS](https://modis.gsfc.nasa.gov/), [Sentinel](https://www.esa.int/Applications/Observing_the_Earth/Copernicus/The_Sentinel_missions), and [Landsat](https://science.nasa.gov/mission/landsat/) have made data freely available, democratizing access to timely satellite RS images of the entire planet. Meanwhile, cloud providers like AWS and Google Cloud have gone so far as to store satellite data, further accelerating the [global usage of these images](http://doi.org/10.5194/isprs-archives-XLIII-B3-2022-597-2022). For example, the Copernicus Sentinel-2 mission includes two polar-orbiting satellites able to re-observe the same area every 5 days. Sentinel-2 images are free and can be accessed, processed, and downloaded through different Python APIs (e.g., [Sentinel Hub, openEO](https://dataspace.copernicus.eu/news/2024-10-9-comparing-openeo-and-sentinel-hub-apis).

Modern EO industry is undergoing an undeniable expansion due to the increasing availability of RS data products in the [global market](ttps://dataspace.copernicus.eu/sites/default/files/media/files/2025-07/0930_terrawatch_the_state_of_earth_observation_forpublication.pdf). It is becoming more affordable to put satellites into space, driven by technological advances in rocket launches and the [miniaturization of payloads](https://doi.org/10.1109/JPROC.2018.2806218). The ability to monitor our planet in high-resolution, on-demand, and in near real-time is driven by new technologies like SmallSats and [onboard AI](http://doi.org/10.1109/CVPRW53098.2021.00230). In the next five years alone (2026–2029), 1,158 new EO satellites are expected to launch. We have already reached a point where major constellations like Sentinel, Landsat, and PlanetScope generate an estimated 50TB of data every single day. This exponential growth has created a massive challenge: transforming this overwhelming flood of raw pixels into usable information to meet the need for scalable downstream insights.

The research community of geoscience and remote sensing has been applying a vast variety of algorithmic techniques for [over 50 years](https://docs.lib.purdue.edu/larstech/129). Until a decade ago, common pattern recognition tasks (e.g., extraction of building footprints, identifying vegetation in the urban areas, etc.) were arduous tasks often requiring labor-intensive manual digitization or limited by the constraints of traditional pixel-based methods. Then, in 2012, the “deep learning revolution” - marked by the success of [AlexNet](https://dl.acm.org/doi/10.5555/2999134.2999257)—opened up an entirely novel frontier of automatic and efficient algorithms that could be applied to satellite imagery with state-of-the-art results [A. Krizhevsky, 2012]. 







 These models significantly improve downstream tasks such as land-cover mapping, semantic segmentation, and change detection, though they require distributed high-performance computing strategies to manage the extensive training costs associated with massive datasets. Recent developments increasingly emphasize multimodal and generative capabilities; for instance, TerraMind employs a unique dual-scale architecture processing both token-level and pixel-level inputs to directly synthesize EO data, enabling 'Thinking-in-Modalities' (TiM) for end-to-end image regeneration and enhanced analysis.

The availability of large volumes of heterogeneous, often unlabeled data, coupled with the synergies of multi-source integration, aligns well with recent trends in generative visual AI. Foundational models, originally popularized for natural language processing, have become central to Earth Observation (EO) research and operational pipelines. Prominent Geospatial Foundation Models (GFMs) such as Prithvi-EO-2.0 and TerraMind leverage architectures defined by massive parameter counts and large-scale pretraining to learn transferable representations. Drawing on progress in vision–language learning, these models significantly boost performance in downstream tasks—such as land-cover mapping, semantic segmentation, and change detection—particularly in scenarios where labeled data is sparse. Furthermore, because Transformer backbones like Vision Transformers (ViTs) follow predictable scaling laws, the use of distributed hardware has become critical for timely and efficient pretraining.

In this context, many challenges remain, particularly in bridging the gap between controlled benchmark evaluations and the complex requirements of real-world application [C. Butsko et al., 2025]. The Earth Observation (EO) community needs to transition Foundation Models (FMs) from research prototypes into operational, trustworthy tools that ensure physical consistency—such as adherence to spectral smoothness and energy conservation—while maintaining the computational efficiency required for edge deployment,,. The information contained in remote sensing data is an irreplaceable asset for tackling challenges as wide-ranging as quantifying climate change impacts, predicting crop yields, managing disasters like floods, and calculating progress toward the Sustainable Development Goals. However, the field must address hurdles such as limited labeled data, geographic bias where models fail to generalize to unseen regions, and the inadequacy of standard benchmarks to reflect operational nuances. The outlook is transformative, envisioning a shift from static pipelines to dynamic 'agentic AI' systems capable of autonomous reasoning, real-time decision-making, and intrinsic motivation-driven learning,,. Future progress will rely on fusing physical laws with data-driven models to enhance feature fidelity and fostering interdisciplinary collaboration to bridge data and computility islands, thereby democratizing access to Earth science insights."


Surbhi Embeddings
Although most of the existing land-cover products have
been generated with Sentinel-2 image time series, recent
advances in geospatial foundation models, such as Temporal
Embeddings of Surface Spectra for Earth Representation
and Analysis (TESSERA) [22] and AlphaEarth Foundations
[23], offer a fundamentally different paradigm known as
embeddings-as-data: precomputed, generic, task-agnostic features
that can be easily adapted with lightweight heads by
providing learned embeddings from multi-temporal, multisource
Earth observation data at 10 m resolution. These models
leverage self-supervised learning to create robust, analysisready
feature representations that achieve high accuracy with
minimal labeled data, potentially overcoming the limitations
of both synthetic and map-based training approaches for largescale
built-up area characterization.




# References














[G. Schumann] Guy Schumann, "Every drop counts: How space tech innovations are revolutionising Earth observation", https://www.innovationnewsnetwork.com/every-drop-counts-how-space-tech-innovations-are-revolutionising-earth-observation/58641/ 





[C. Butsko et al., 2025] C. Butsko, K. V. Tricht, G. Tseng, et al., "Deploying Geospatial Foundation Models in the Real World: Lessons from WorldCereal", 2025, https://doi.org/10.48550/arXiv.2508.00858