# Wisconsin Breast Cancer Clustering Analysis 🧬

[![TR](https://img.shields.io/badge/Lang-TR-red.svg)](#türkçe) [![EN](https://img.shields.io/badge/Lang-EN-blue.svg)](#english)

### Dosya Yapısı
- [**wbc_clustering_analysis.ipynb**](./wbc_clustering_analysis.ipynb): Veri ön işleme, K-Means & DBSCAN modellemeleri ve PCA görselleştirmelerini içeren Python Notebook dosyası.
- [**WBC-Kümeleme-Raporu.pdf**](./WBC-Kümeleme-Raporu.pdf): Analiz süreçlerini ve çıktılarını anlatan proje raporu.
- [**wdbc.data**](./wdbc.data): Projede kullanılan ana veri seti.
- [**wdbc.names**](./wdbc.names): Veri seti özelliklerinin detaylarını içeren bilgi dosyası.

### Repository Structure
- [**wbc_clustering_analysis.ipynb**](./wbc_clustering_analysis.ipynb): Python Notebook containing data preprocessing, K-Means & DBSCAN modeling, and PCA visualizations.
- [**WBC-Kümeleme-Raporu.pdf**](./WBC-Kümeleme-Raporu.pdf): The project report explaining the analysis processes and outputs.
- [**wdbc.data**](./wdbc.data): The main dataset used in the analysis.
- [**wdbc.names**](./wdbc.names): Metadata file detailing the dataset's features.
---

## 🇹🇷 Türkçe

### Proje Hakkında
Bu proje, Wisconsin Breast Cancer (WDBC) veri kümesi temel alınarak denetimsiz öğrenme yaklaşımıyla gerçekleştirilmiş bir kümeleme analizidir. Projenin amacı, kanser teşhisiyle ilişkili sayısal özellikleri kullanarak örnekleri benzer özelliklerine göre gruplandırmak ve elde edilen kümelerin yapısını incelemektir.


### Veri Kümesi ve Ön İşleme
- Analizde 30 adet sayısal özellik içeren `wdbc.data` kullanılmıştır ve veride eksik değer bulunmadığı doğrulanmıştır.
- Özelliklerin farklı ölçeklerde olması nedeniyle veri kümesindeki tüm değişkenler StandardScaler yöntemiyle ölçeklendirilmiştir.

### Kullanılan Yöntemler
- **K-Means Kümeleme:** Kümeleme işlemi için K-ortalamalar (K-Means) algoritması tercih edilmiştir. Uygun küme sayısı (k) dirsek (elbow) yöntemiyle belirlenmiştir.
- **DBSCAN Kümeleme:** Alternatif bir yöntem olarak DBSCAN kümeleme analize dahil edilmiştir.
- **Silhouette Skoru:** Kümelerin ayrışma düzeyini değerlendirmek için Silhouette skoru hesaplanmıştır.
- **PCA (Temel Bileşenler Analizi):** Verilerin 2 boyutta (PCA 2D) görselleştirilmesi için kullanılmıştır.

### Bulgular ve Sonuç
- Elde edilen kümelerin, veri kümesindeki benign (iyi huylu) ve malignant (kötü huylu) örneklerle genel olarak örtüştüğü gözlenmiştir.
- Önişleme adımlarının ve uygun küme sayısının belirlenmesinin analiz kalitesine önemli ölçüde katkı sağladığı ortaya konmuştur.

### Dosya Yapısı
- `wbc_clustering_analysis.ipynb`: Veri ön işleme, K-Means & DBSCAN modellemeleri ve PCA görselleştirmelerini içeren Python Notebook dosyası.
- `WBC-Kümeleme-Raporu.pdf`: Analiz süreçlerini ve çıktılarını anlatan proje raporu.
- `wdbc.data`: Projede kullanılan ana veri seti.
- `wdbc.names`: Veri seti özelliklerinin detaylarını içeren bilgi dosyası.

---

## 🇬🇧 English

### About the Project
This project performs a clustering analysis using an unsupervised learning approach based on the Wisconsin Breast Cancer (WDBC) dataset. The aim is to group instances based on their similarities using various numerical features related to cancer diagnosis and to examine the structure of the obtained clusters.


### Dataset & Preprocessing
- The analysis utilizes the `wdbc.data` dataset, which contains 30 numerical features with no missing values.
- Because features are on different scales, all variables were scaled using the StandardScaler method.

### Methodology
- **K-Means Clustering:** The K-Means algorithm was chosen for the clustering process. The appropriate number of clusters (k) was determined using the elbow method.
- **DBSCAN Clustering:** DBSCAN clustering was included in the analysis as an alternative method.
- **Silhouette Score:** The Silhouette score was calculated to evaluate the level of separation between clusters.
- **PCA (Principal Component Analysis):** Used to reduce and visualize the data in 2 dimensions (PCA 2D).

### Findings & Conclusion
- It was observed that the resulting clusters generally overlap with the benign and malignant instances in the dataset.
- The results demonstrate that preprocessing steps and determining the appropriate number of clusters significantly contribute to the quality of the analysis.

### Repository Structure
- `wbc_clustering_analysis.ipynb`: Python Notebook containing data preprocessing, K-Means & DBSCAN modeling, and PCA visualizations.
- `WBC-Kümeleme-Raporu.pdf`: The project report explaining the analysis processes and outputs.
- `wdbc.data`: The main dataset used in the analysis.
- `wdbc.names`: Metadata file detailing the dataset's features.
