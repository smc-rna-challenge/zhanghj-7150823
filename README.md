SMC-RNA Challenge Entry: zhanghj-7150823
========================================================

This is a CWL workflow which was submitted to the [SMC-RNA Challenge][smcrna] in the isoform quantification category.

Example and reference data files are stored on [Synapse][data] and are
defined in synapse_inputs.json.  
A Synapse user account is required to access data from Synapse.

Usage
--------------------------------------------------------

```bash
# Clone this repo
git clone https://github.com/smc-rna-challenge/zhanghj-7150823
cd zhanghj-7150823

# Install the requirements
pip install -r requirements.txt

# Download the test data to ./data
# You'll need a synapse.org account.
python download.py

# Run the workflow
cwltool main.cwl
```

Resource Usage
--------------------------------------------------------

Most SMC-RNA entries were tested on machines with 16 vCPUs and 60 GB of RAM.
Many entries did not use the full amount of resources.
Some required more memory and were allowed 104 GB of RAM.


Docker images
--------------------------------------------------------


- [quay.io/smc-rna-challenge/zhanghj-7150823-kallisto:1.0.0](https://quay.io/smc-rna-challenge/zhanghj-7150823-kallisto:1.0.0)





Details
========================================================

Challenge participants were asked to complete a quiz to describe some of the
details about their entry:



#### What methods does the tool use?
Pseudo-alignment



#### What alignment algorithms does the tool use?
Kallisto



#### Are there non-default parameters used for the alignment algorithms?
No





#### Are there other inputs other than sequencing reads and gene annotation?
No













#### Does your method require isoform models to be supplied or is it reference free, able to construct transcripts de novo?
Not applicable to my method.





#### Other than transcript models, does your method make use of any prior information not available in the data? If so, does it use:
The method does not make use of prior knowledge in any form.



#### Is your approach a stand-alone algorithm or would you consider it to be an ensemble of multiple methods that are later combined in some way?
Stand-alone method



#### Does your method require any specific parameters for tuning (e.g. mean and standard deviation of expected fragment sizes)?
No



#### Do you anticipate your algorithm would need to be parameterized for different read-lengths?
Yes





#### If your method detects cancer-associated fusions, does it filter out those found in normal (or other control) samples?
No









#### If your method infers expression levels, does it simultaneously identify transcripts and their expression levels or does it perform these steps sequentially?
Simultaneously



#### Is your method alignment independent?
Yes



#### Does your method use the quality of the read mapping at all (e.g. filter out poorly mapped reads)?
Yes



#### Does your method use information about strand-specific sequences?
Yes



#### Does your method output transcript-length- and library size- adjusted estimates of abundance (such as RPKM, FPKM, or TPM)?
Yes





[smcrna]: https://www.synapse.org/#!Synapse:syn2813589/wiki/401435
[data]: https://www.synapse.org/#!Synapse:syn9878767
