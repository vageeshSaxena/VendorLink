# VendorLink: A (Semi-)Supervised NLP approach for Identifying & Linking Vendor Migrants & Aliases on Darknet Markets
The anonymity on the Darknet allows vendors to stay undetected by using multiple vendor aliases or frequently migrating between markets. Consequently, illegal markets and their connections are challenging to uncover on the Darknet. To identify relationships between illegal markets and their vendors, we propose VendorLink, an NLP-based approach that examines writing patterns to verify, identify, and link unique vendor accounts across text advertisements (ads) on seven public Darknet markets. In contrast to existing literature, VendorLink utilizes the strength of supervised pre-training to perform closed-set vendor verification, open-set vendor identification, and low-resource domain adaption tasks. Altogether, our approach can help Law Enforcement Agencies (LEA) make more informed decisions by verifying and identifying migrating vendors and their potential aliases with state-of-the-art (SOTA) performance on both existing and emerging low-resource (LR) Darknet markets.

![(i) Closed-Set Vendor Verification Task: A supervised-pretraining task that utilizes closed-set classification to verify unique vendor migrants across known markets (ii) Open-set Vendor Identification Task: An open-set text-similarity task that utilizes embeddings from the pre-trained classifier to verify known vendors and identify potential-aliases (iii) Low-resource domain adaptation task: A knowledge-transfer task to adapt new domain knowledge and verify migrants across low-resource emerging markets.](Images/vendorLink.png)
(i) Closed-Set Vendor Verification Task: A supervised-pretraining task that utilizes closed-set classification to verify unique vendor migrants across known markets (ii) Open-set Vendor Identification Task: An open-set text-similarity task that utilizes embeddings from the pre-trained classifier to verify known vendors and identify potential-aliases (iii) Low-resource domain adaptation task: A knowledge-transfer task to adapt new domain knowledge and verify migrants across low-resource emerging markets.

# Dataset
For reproducibility purposes, we conduct our analyses on publically available Darknet advertisements datasets from Agora, Alphabay, Dreams, Traderoute, Valhalla, and Berlusconi non-anonymous markets. All the datasets are hosted by IMPACT cyber trust portal and Kaggle. They can be downloaded through the links below:

1) [Alphabay marketplace, 2017-18](https://github.com/user/repo/blob/branch/other_file.md) : AlphaBay was an online darknet market launched in September 2014, pre-launched in November 2014, and officially launched on December 22, 2014, an onion service of the Tor network. In 2017, it was shut down after a law enforcement action as a part of Operation Bayonet (along with Hansa market) in the United States, Canada, and Thailand. At its demise in July 2017, AlphaBay had over 400,000 users. The non-anonymous dataset was collected from a publicly available website over two and a half years, 2014-2017. The dataset consists of 1,771,258 advertisements from 6,250 unique vendors.
2) [Dream, Traderoute, Berlusconi and Valhalla marketplaces, 2017-2018](http://dx.doi.org/10.23721/116/1503879) : Dream Market was an online darknet market founded in late 2013. Following the seizures and shutdowns of the AlphaBay and Hansa markets, Traderoute and Dream Market became predominant marketplaces on the Dark Web. During the time, Dream Market was estimated as the second-largest darknet marketplace, with AlphaBay being the largest and Hansa the third-largest. After Operation Bayonet, many vendors and buyers from AlphaBay and Hansa communities migrated to Dream Market. At the time, Dream Market was reported to have 57,000 listings for drugs and 4,000 listings for opioids. The marketplace sold a variety of content, including drugs, stolen data, and counterfeit consumer goods, all using cryptocurrency. In addition, dream provided an escrow service, with disputes handled by staff. The market also had accompanying forums hosted on a different URL, where buyers, vendors, and other community members could interact. Eventually, Administrator and prolific vendor Gal Vallerius was arrested in August 2017 and the site shut down on April 2019. The non-anonymous Dream dataset collected by Carnegie Mellon University has 1,816,854 listings by 5,780 vendors between 2016 -18.
3) [Silk Road marketplace, 2012-13](http://dx.doi.org/10.23721/116/1406256) : Silk Road-1 was the first modern online black market notoriously known for selling illegal drugs. The website was first launched in February 2011, with a limited number of new seller accounts available. Later, new sellers acquired other accounts in an auction for a fixed fee. Finally, on October 2013, the FBI seized the website and arrested Ross Ulbricht for being the site's pseudonymous founder, "Dread Pirate Roberts." The non-anonymous Silk Road-1 dataset from Carnegie Mellon University has 1,065,810 listings by 2,872 vendors between 2012-13.
4) [Agora marketplace, 2014-15](https://www.kaggle.com/datasets/philipjames11/dark-net-marketplace-drug-data-agora-20142015) : Agora was operated on the Tor network between 2013-15. After the demise of Evolution and Silk Road 2.0, Agora became the largest marketplace in March 2015. The Kaggle data parse contains drugs, weapons, books, and services. Duplicate listings have been removed, and prices have been averaged for duplicates. The data is in a CSV file and has over 100,000 unique listings.





