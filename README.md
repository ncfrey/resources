# A Highly Opinionated List of Open Source Materials Informatics Resources
A list of resources for [getting started](#getting-started), [blogs, newsletters, and podcasts](#blogs-newsletters-and-podcasts), [python tools](#python-tools), and [databases](#databases) for [materials informatics](https://citrine.io/what-is-materials-informatics/). If you think there's a great resource missing, read the [contribution guide](https://github.com/ncfrey/resources/blob/main/CONTRIBUTING.md) and [open a pull request](https://github.com/ncfrey/resources/pulls) or [create an issue](https://github.com/ncfrey/resources/issues) and I'll be happy to add it. This list is in no way comprehensive, it's simply a collection of resources I've found extremely helpful in my own research. This field is rapidly evolving and I've tried to focus on materials-specific resources, rather than cover the constantly changing cutting-edge of data science tools. I have included some foundational tools that are prerequisites for most of the other resources. This list is inspired by Pat Walters' excellent [list of resources](https://github.com/PatWalters/resources) for cheminformatics. Chemistry, the so-called "central science," is in many ways leading the charge when it comes to applying machine learning to science, so it doesn't hurt to be familiar with the progress in the field.

## Getting started
- [What is materials informatics?](https://citrine.io/what-is-materials-informatics-blog/) - This blog post from Citrine does a really nice job summarizing what materials informatics is and why it's worth doing.

- [Machine Learning for Materials Scientists: An Introductory Guide toward Best Practices](https://pubs.acs.org/doi/abs/10.1021/acs.chemmater.0c01907) - There are too many reviews and perspectives on ML for materials science to count; I like this one because it includes [example code and notebooks](https://github.com/anthony-wang/BestPractices) and plenty of helpful tables with references to databases and work in the field. If you read this paper and work through the examples, you'll have a solid foundation for doing materials informatics research.

- [Matminer Tutorials](https://nbviewer.jupyter.org/github/hackingmaterials/matminer_examples/blob/master/matminer_examples/index.ipynb) - The Matminer tutorial series uses interactive Jupyter notebooks to walk through the basic steps of materials informatics: data retrieval, featurization, machine learning, and data evaluation/visualization.

- [Materials Project Workshop](https://workshop.materialsproject.org/#workshop-videos) - This fantastic three day workshop offered annually by the wonderful folks at the [Materials Project](https://materialsproject.org/) covers introductions to Python, Jupyter notebooks for data science, MongoDB for databases, and using the full stack of Materials Project software for computational materials science. There are [lecture videos](https://www.youtube.com/watch?v=vga6eV3IAac&list=PLTjFYVNE7LTiuOK8Re7ltY0a3OHFcQhAE) and [interactive notebooks](https://github.com/materialsproject/workshop/) accompanying each lesson. Appropriate for anyone with an interest in computational materials, no need to be a Python wizard.

## Blogs, newsletters, and podcasts
- [My blog](https://medium.com/@ncfrey) - I post occasionally about my own research in materials informatics and materials physics. 

- [Citrine Blog](https://citrine.io/success/blog/) - There are some good posts here about challenges in the field, as well as [specific case studies](https://citrine.io/category/case-studies/) and [white papers](https://citrine.io/category/white-papers/)

- [Citrine Newsletters](https://citrine.io/success/newsletters/) - A great way to stay up to date with papers in the field, the weekly research newsletter includes reader contributions of relevant papers and job openings.

- [Citrine Podcast](https://citrine.io/success/podcasts/) - There are only a few episodes, but they include some great insights from folks in academia, industry, and even government.

- [Materialism Podcast](https://materialismpodcast.com/episode_list.html) - Materialism is a great podcast about general topics in materials science. Check out episode #20 for an informatics focus. Caveat that I strongly disagree with their intro :sweat_smile:

- [ML4Sci](https://ml4sci.substack.com/) - A newsletter that covers all applications of machine learning to applied science, including materials.

## Python Tools
- [Jupyter](https://jupyter.org/) - Project Jupyter is the de facto standard for doing data science in an interactive, web-based interface. A common theme among these resources is that the best ones will always be accompanied by example code and Jupyter notebooks. Advantages: great for rapid iteration and experimentation (science). Disadvantages: not great for reproducibility, deployment in production, and robustness (engineering).  

- [Deepnote](https://deepnote.com/) - There are lots of new notebook environments popping up trying to address the disadvantages of Jupyter. Deepnote allows real-time collaboration and runs in the cloud. [Google Colab](https://colab.research.google.com/), [CoCalc](https://cocalc.com/app), and [Paperspace Gradient](https://gradient.paperspace.com/) are other cloud-based notebook environments for ML.

- [Gradio](https://gradio.app/) - Lightweight application for building and sharing web interfaces to your ML models. 

### Computational materials workflow libraries
- [Pymatgen](http://pymatgen.org/) - All-purpose code for representing materials structures, interfacing with electronic structure codes, and analyzing materials data.

- [MP Infrastructure](https://materialsproject.org/infrastructure) - Built on pymatgen, [custodian](https://materialsproject.github.io/custodian), [fireworks](https://materialsproject.github.io/fireworks), and [atomate](https://hackingmaterials.github.io/atomate), these codes enable automated, high-throughput calculations and analysis of materials.

- [AiiDA](http://www.aiida.net/) - Automated computational materials science workflows with robust tracking of data provenance.

- [ASE](https://wiki.fysik.dtu.dk/ase) - Simulation environment for materials and molecules.

### Materials informatics libraries
- [Matminer](https://hackingmaterials.lbl.gov/matminer/) and [Automatminer](https://github.com/hackingmaterials/automatminer) - Automated generation of descriptors from material structures and compositions, as well as ML model training and evaluation.

- [PUMML](https://github.com/ncfrey/pumml) - Semi-supervised materials machine learning (e.g. to predict synthetic accessibility) 

- [pytopomat](https://github.com/ncfrey/pytopomat) - Workflows for high-throughput band topology calculations.

- [MAML](https://github.com/materialsvirtuallab/maml) - All-purpose library for materials ML.

- [MEGNet](https://github.com/materialsvirtuallab/megnet) - Graph networks for molecules and crystals.

- [DeepChem](https://deepchem.io/) - Deep learning for the sciences. Support for PyTorch and TensorFlow, focused on chemical and life sciences with increasing support for materials science.

### Visualization and data sharing
- [Crystal Toolkit](https://github.com/materialsproject/crystaltoolkit) - Interactive web app for visualizing materials science data.

- [SUMO](https://smtg-ucl.github.io/sumo/index.html) - Plotting tools for electronic structure calculation data.

- [MPContribs](https://mpcontribs.org/) - Contribute theoretical and experimental datasets directly to the Materials Project, sharing your data with 100,000+ users and making it easily accessible through the web interface and API.

- [MDF](https://materialsdatafacility.org/) - A way to publish your own materials datasets with an API for accessing them.

## Databases
- [Materials Project](https://materialsproject.org/) - Over 130,000 inorganic compounds and 49,000 molecules and counting, with calculated phase diagrams, structural, thermodynamic, electronic, magnetic, and topological properties.

- [OQMD](http://oqmd.org/) - 815,000+ materials with calculated thermodynamic and structural properties.

- [ICSD](https://icsd.nist.gov/) - 210,000+ inorganic crystal structures from literature. Requires a subscription.

- [JARVIS](https://jarvis.nist.gov/) - Includes calculated materials properties, 2D materials, and tools for ML and high-throughput tight-binding.

- [C2DB](https://cmr.fysik.dtu.dk/c2db/c2db.html) - Calculated properties for thousands of 2D materials.

- [AFLOW](http://www.aflowlib.org/) - Millions of materials and calculated properties, focusing on alloys.

- [Materials Cloud](https://www.materialscloud.org/explore/menu) - A collection of databases curated by the Marzari group at EPFL.

- [NOMAD](https://nomad-lab.eu/prod/rae/gui/search) - Repository for materials data following the [FAIR](https://doi.org/10.1557/mrs.2018.208) principles. 

- [Citrination](https://citrination.com) - Contributed and curated datasets from Citrine.

- [MPDS](https://mpds.io/#start) - An initiative to scrape data from literature and make it machine readable.



