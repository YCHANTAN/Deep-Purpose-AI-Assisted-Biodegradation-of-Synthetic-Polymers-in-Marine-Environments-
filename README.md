# AI-Assisted Biodegradation of Synthetic Polymers in Marine Environments 🌊🧪

📌 Project Overview
This research explores the intersection of Machine Learning and Environmental Microbiology to solve the marine plastic crisis. By integrating traditional statistical clustering with cutting-edge Deep Learning (DTI), the project identifies which synthetic polymers are most susceptible to microbial attack and predicts the binding affinity of marine-derived enzymes.

🚀 Key Features
- Structural Clustering: K-Means clustering of synthetic polymers based on Molecular Weight and Hydrophobicity.
- Virtual Screening: Utilizes the DeepPurpose framework to simulate interactions between plastic backbones and microbial enzymes.
- Hybrid Neural Network: Employs a Message Passing Neural Network (MPNN) for polymer graph encoding and a Convolutional Neural Network (CNN) for protein sequence analysis.
- Affinity Prediction: Generates a "Biodegradation Score" ($pK_d$) to identify lead candidate "Super-Degraders" for targeted bioremediation.

🛠️ Tech Stack
- Language: Python (3.12+ recommended for Colab)
- Deep Learning: PyTorch, DeepPurpose
- Cheminformatics: RDKit
- Data Analysis: Pandas, NumPy, Scikit-Learn
- Visualization: Matplotlib, Seaborn

📊 Data & Methodology
1. Polymer Characterization
Analyzing 44+ synthetic polymers (PVA, PEG, PAA) through chemical descriptor extraction.

2. Microbial Bioprospecting
Cross-referencing global catalogs of 400+ plastic-degrading microbes isolated from marine environments.

3. MPNN-CNN Interaction Modeling
The core of the project uses a pre-trained MPNN_CNN_BindingDB model.
- MPNN: Captures the atomic connectivity and bond types of the polymer.
- CNN: Learns the amino acid patterns (motifs) in the enzyme sequence.

📈 Results Summary
- Top Interaction Score: 17.0666 (Predicted $pK_d$).
- Lead Candidate: Carboxyl-rich backbones paired with Cluster-1 Marine Bacteria.
- Key Insight: The "PVA Advantage"—Poly(vinyl alcohol) demonstrates superior bioavailability due to high hydroxyl density and chain accessibility.

⚙️ Installation & Usage
To run the deep learning screening, it is recommended to use Google Colab:
1. Upload your .xlsx and .xls datasets.
2. Install dependencies:
   pip install DeepPurpose rdkit scikit-learn==1.2.2 numpy==1.23.5
