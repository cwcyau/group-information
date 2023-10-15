# Research Projects

## Foundations of Machine Learning

I am generally interested in how to build machine learning (ML) models with more *realistic* underlying assumptions for applied scientific applications. A general feature of machine learning development is that it is often undertaken by individuals who have had very little background in applied sciences. As a consequence, ML methods can often be somewhat divorced from their potential real world use by stylising the problem into a form which is mathematically or computationally convenient and/or elegant but not practicable for end-users. Implicit assumptions can also be made which are unrealistic, e.g. the amount of available data or assuming that the model can be used independently of human decision making. 

There are two major themes aspects in which I am currently interested: 

### Feature-level interpretability

In the biological sciences, molecular tools are used to probe cellular and physiological machinery to understand their normal, diseased and perturbed (e.g. genetic modification, chemical stimulation) behaviours. Validation of *biological mechanism* relies on being able to measure biophysical quantities (e.g. DNA, mRNA, proteins, metabolites, etc). True interpretation can *only* be achieved in terms of these physical objects. In contrast, in recent machine learning development, the literature on explainability and interpretability has often drifted into the abstract and it can be difficult to understand representations in terms of their relationship to physically measureable quantities. 

I am interested in the specification of machine learning which possess *feature-level interpretability* where representations and post-hoc interpretation are explicitly tied to the specification of measurable input features. This work connects machine learning with explicit mechanistic models (e.g. differential equations) and is often overlooked as mainstream ML developers typically focus on ML first, not the details of the application.

### Stability of machine learning models

Unstable machine models are problematic in critical applications, such as in medical devices, where medical device regulation imposes certain safety and assurance conditions on manufacturers. Instability can occur due to a number of factors including (i) model misspecification, (ii) inadequate inference, and (iii) data distribution shifts during real runtime. The effect is that ML models could give wildly different outputs for inputs which are potentially similar. 

I am interested in understanding if there are specifications of machine learning models which can explicitly help to avoid common instability issues and their implications for medical device regulation. This work would require developing an understanding of (what are typically considered to be) downstreet regulatory issues, can impact on the design of ML systems at the fundamental level.

## Applications

### Foundation Models for Multiple Long-Term Conditions research

I am co-lead in two national consortia ([MuM-PreDicT](https://mumpredict.org/) (pregnancy) and [OPTIMAL] (https://www.birmingham.ac.uk/research/applied-health/research/optimal/index.aspx) (ageing) which are studying the health outcomes of individuals with two or more chronic health conditions in the UK. This research predominately uses electronic health records held in large repositories (e.g. [CPRD](https://cprd.com/)). These databases are highly-protected and access restricted to vetted users with a genuine and approved research plan. This stringent approach makes the widespread use of this data difficult outside of a relatively small community of researchers and industry. We are interested in building [foundation models](https://en.wikipedia.org/wiki/Foundation_models) using these databases which could serve as a protected proxy allowing access to the knowledge contained in the database but without the possibility of revealing individual health records. This capability could then enable the production of clinical prediction models for a variety of conditions including women's health issues of unmet need. This application links to the *stability of machine learning models* work described above.

### Multimodal Cancer Predictive Models

As Bioinformatics & Machine Learning Research Network Lead for [Genomics England](https://www.google.com/search?q=genomics+england&rlz=1C5CHFA_enGB984GB984&oq=genomics+england&gs_lcrp=EgZjaHJvbWUyCQgAEEUYORiABDIGCAEQIxgnMgkIAhAjGCcYigUyBwgDEAAYgAQyBggEEEUYPDIGCAUQRRg8MgYIBhBFGDwyBggHEEUYQagCALACAA&sourceid=chrome&ie=UTF-8), I am interested in utilising their multimodal dataset consisting of whole cancer genomes and pathology images to develop clinical prediction models that combines clinical, genetic and tissue imaging information to provide an indication of possible prognostic outcomes. This application links to the *feature-level interpretability* work discussed above.

### Multimodal Vaccine Data Integration

With [Daniel O'Connor](https://www.ovg.ox.ac.uk/team/daniel-oconnor), we are interested in developing methods to integrate lots of molecular data collected from vaccine trials and studies to yield new insights into vaccine effectiveness. Each study is relatively small and so pooling of information across different experimental studies to yield new insights is challenging and requires algorithmic automation as manual curation is too cumbersome. I am interested in the meta-learning problem of combining data collected across heterogeneous studies and experimental designs and how the automation process allows for this to be done, not once, but repeatedly. This application links to the *feature-level interpretability* work discussed above.
