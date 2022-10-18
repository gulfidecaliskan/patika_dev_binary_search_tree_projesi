# patika_dev_binary_search_tree_projesi
Bu proje [Patika Dev'in](https://www.patika.dev/) Veri Yapıları ve Algoritmalar eğitiminin 3. projesidir.

## [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.
### Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

- Root olarak 7'yi seçtim. Siz istediğinizi seçebilirsiniz. Dikkate almanız gereken nokta root'a göre diğer düğümleri yerleştirmelisiniz. Eğer düğüm roottan büyükse sağa eğer düğüm roottan küçükse sola gelmeli.


|           Açıklama          |   |   |   |
|:---------------------------:|:-:|:-:|:-:|
| Root'u 7 olarak belirledik. |   | 7 |   |

- 5'i root'a göre konumlandırdık.

|  Açıklama  |   |   |   |
|:----------:|:-:|:-:|:-:|
|            |   |   | 7 |
|            |   | / |   |
| 5 ekledik. | 5 |   |   |

- 1'i root'a göre konumlandırdık.

|  Açıklama  |   |   |   |   |   |
|:----------:|---|---|:-:|:-:|:-:|
|            |   |   |   |   | 7 |
|            |   |   |   | / |   |
|            |   |   | 5 |   |   |
|            |   | / |   |   |   |
| 1 ekledik. | 1 |   |   |   |   |

- 8'i root'a göre konumlandırdık.

|  Açıklama  |   |   |   |   |   |   |   |
|:----------:|---|---|:-:|:-:|:-:|---|---|
|            |   |   |   |   | 7 |   |   |
|            |   |   |   | / |   | \ |   |
| 8 ekledik. |   |   | 5 |   |   |   | 8 |
|            |   | / |   |   |   |   |   |
|            | 1 |   |   |   |   |   |   |

- 3'ü root'a göre konumlandırdık.

|  Açıklama  |   |   |   |   |   |   |   |
|:----------:|---|---|:-:|:-:|:-:|---|---|
|            |   |   |   |   | 7 |   |   |
|            |   |   |   | / |   | \ |   |
|            |   |   | 5 |   |   |   | 8 |
|            |   | / |   |   |   |   |   |
|            | 1 |   |   |   |   |   |   |
|            |   | \ |   |   |   |   |   |
| 3 ekledik. |   |   | 3 |   |   |   |   |

- 6'yı root'a göre konumlandırdık.

|  Açıklama  |   |   |   |   |   |   |   |
|:----------:|---|---|:-:|:-:|:-:|---|---|
|            |   |   |   |   | 7 |   |   |
|            |   |   |   | / |   | \ |   |
|            |   |   | 5 |   |   |   | 8 |
|            |   | / |   | \ |   |   |   |
| 6 ekledik. | 1 |   |   |   | 6 |   |   |
|            |   | \ |   |   |   |   |   |
|            |   |   | 3 |   |   |   |   |

- 0'ı root'a göre konumlandırdık.

|  Açıklama  |   |   |   |   |   |   |   |   |   |
|:----------:|---|---|---|---|:-:|:-:|:-:|---|---|
|            |   |   |   |   |   |   | 7 |   |   |
|            |   |   |   |   |   | / |   | \ |   |
|            |   |   |   |   | 5 |   |   |   | 8 |
|            |   |   |   | / |   | \ |   |   |   |
|            |   |   | 1 |   |   |   | 6 |   |   |
|            |   | / |   | \ |   |   |   |   |   |
| 0 ekledik. | 0 |   |   |   | 3 |   |   |   |   |

- 9'u root'a göre konumlandırdık.

|  Açıklama  |   |   |   |   |   |   |   |   |   |   |   |
|:----------:|---|---|---|---|:-:|:-:|:-:|---|---|---|---|
|            |   |   |   |   |   |   | 7 |   |   |   |   |
|            |   |   |   |   |   | / |   | \ |   |   |   |
|            |   |   |   |   | 5 |   |   |   | 8 |   |   |
|            |   |   |   | / |   | \ |   |   |   | \ |   |
| 9 ekledik. |   |   | 1 |   |   |   | 6 |   |   |   | 9 |
|            |   | / |   | \ |   |   |   |   |   |   |   |
|            | 0 |   |   |   | 3 |   |   |   |   |   |   |

- 4'ü root'a göre konumlandırdık.

|  Açıklama  |   |   |   |   |   |   |   |   |   |   |   |
|:----------:|---|---|---|---|:-:|:-:|:-:|---|---|---|---|
|            |   |   |   |   |   |   | 7 |   |   |   |   |
|            |   |   |   |   |   | / |   | \ |   |   |   |
|            |   |   |   |   | 5 |   |   |   | 8 |   |   |
|            |   |   |   | / |   | \ |   |   |   | \ |   |
|            |   |   | 1 |   |   |   | 6 |   |   |   | 9 |
|            |   | / |   | \ |   |   |   |   |   |   |   |
|            | 0 |   |   |   | 3 |   |   |   |   |   |   |
|            |   |   |   |   |   | \ |   |   |   |   |   |
| 4 ekledik. |   |   |   |   |   |   | 4 |   |   |   |   |

- 2'yi root'a göre konumlandırdık.

|  Açıklama  |   |   |   |   |   |   |   |   |   |   |   |
|:----------:|---|---|---|---|:-:|:-:|:-:|---|---|---|---|
|            |   |   |   |   |   |   | 7 |   |   |   |   |
|            |   |   |   |   |   | / |   | \ |   |   |   |
|            |   |   |   |   | 5 |   |   |   | 8 |   |   |
|            |   |   |   | / |   | \ |   |   |   | \ |   |
|            |   |   | 1 |   |   |   | 6 |   |   |   | 9 |
|            |   | / |   | \ |   |   |   |   |   |   |   |
|            | 0 |   |   |   | 3 |   |   |   |   |   |   |
|            |   |   |   | / |   | \ |   |   |   |   |   |
| 2 ekledik. |   |   | 2 |   |   |   | 4 |   |   |   |   |