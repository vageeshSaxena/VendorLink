# VendorLink: A (Semi-)Supervised NLP approach for Identifying & Linking Vendor Migrants & Aliases on Darknet Markets
The anonymity on the Darknet allows vendors to stay undetected by using multiple vendor aliases or frequently migrating between markets. Consequently, illegal markets and their connections are challenging to uncover on the Darknet. To identify relationships between illegal markets and their vendors, we propose VendorLink, an NLP-based approach that examines writing patterns to verify, identify, and link unique vendor accounts across text advertisements (ads) on seven public Darknet markets. In contrast to existing literature, VendorLink utilizes the strength of supervised pre-training to perform closed-set vendor verification, open-set vendor identification, and low-resource domain adaption tasks. Altogether, our approach can help Law Enforcement Agencies (LEA) make more informed decisions by verifying and identifying migrating vendors and their potential aliases with state-of-the-art (SOTA) performance on both existing and emerging low-resource (LR) Darknet markets.

![(i) Closed-Set Vendor Verification Task: A supervised-pretraining task that performs classification in a closed-set environment setting to verify unique vendor migrants across known markets (ii) Open-set Vendor Identification Task: A text-similarity task in open-set environment setting that utilizes embeddings from the pre-trained classifier to verify known vendors and identify potential-aliases (iii) Low-resource domain adaptation task: A knowledge-transfer task to adapt new domain knowledge and verify migrants in a closed-set environment setting across low-resource emerging markets.](docs/Images/vendorLink.png)
(i) __Closed-Set Vendor Verification Task:__ A supervised-pretraining task that performs classification in a closed-set environment setting to verify unique vendor migrants across known markets (ii) __Open-set Vendor Identification Task:__ A text-similarity task in open-set environment setting that utilizes embeddings from the pre-trained classifier to verify known vendors and identify potential-aliases (iii) __Low-resource domain adaptation task:__ A knowledge-transfer task to adapt new domain knowledge and verify migrants in a closed-set environment setting across low-resource emerging markets.

# Documentation
Detailed documentation on the dataset and how to reproduce the main experimental results can be found [here](https://github.com/vageeshSaxena/VendorLink/blob/main/docs/README.md).



