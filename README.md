# oryantasyon0

import math

# Öklid Mesafesi Hesaplama Fonksiyonu
def euclideanDistance(point1, point2):
    return math.sqrt((point1[0] - point2[0])**2 + (point1[1] - point2[1])**2)

# Noktaların Tanımlanması
points = [(2, 3), (4, 5), (1, 1), (6, 7)]

# Mesafelerin Hesaplanması
distances = []
for i in range(len(points)):
    for j in range(i + 1, len(points)):
        distance = euclideanDistance(points[i], points[j])
        distances.append(distance)

# Minimum Mesafenin Bulunması
min_distance = min(distances)
print("Minimum mesafe:", min_distance)
