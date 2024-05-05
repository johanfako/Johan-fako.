# Johan-fako.
Johan fako GPS revolucion 
import numpy as np
import pandas as pd
import geopandas as gpd
from shapely.geometry import Point
import matplotlib.pyplot as plt

# Predpokladajme, že máme dataset s GPS súradnicami
data = {
    'Latitude': [48.7164, 48.6784, 48.6784],
    'Longitude': [21.2611, 21.2996, 21.2996]
}

# Vytvorenie geografického dataframe
df = pd.DataFrame(data)
gdf = gpd.GeoDataFrame(df, geometry=gpd.points_from_xy(df.Longitude, df.Latitude))

# Vizualizácia bodov
gdf.plot(marker='o', color='red', markersize=50)
plt.show()

# Tu by sa mohol pridať ďalší kód pre pokročilé funkcie, ako sú:
# - Autonómna navigácia
# - Vzdialené snímanie
# - Integrácia s cloudovými službami
# - Hlasovo aktivovaná navigácia
# - a ďalšie inovatívne funkcie

# Tento kód je len príkladom a bude potrebné ho prispôsobiť konkrétnym požiadavkám vášho projektu.
