#  House Price Prediction & Analysis  

## Project Overview  
This project analyzes a **dataset** to uncover the key determinants of housing prices and build predictive models.  

#  Feature Dictionary – House Prices Dataset  

---

##  Identification
| Feature | Type | Description |
|---------|------|-------------|
| **Id** | Integer | Unique identifier for each house. |

---

##  Lot & Location
| Feature | Type | Description |
|---------|------|-------------|
| **MSSubClass** | Categorical (int) | Type of dwelling (e.g., 20 = 1-story, 60 = 2-story). |
| **MSZoning** | Categorical | Zoning classification (Residential, Commercial, etc.). |
| **LotFrontage** | Numeric | Linear feet of street connected to property. |
| **LotArea** | Numeric | Lot size in square feet. |
| **Street** | Categorical | Road access type (Grvl, Pave). |
| **Alley** | Categorical | Alley access (Grvl, Pave, NA if none). |
| **LotShape** | Categorical | Shape of property (Reg = Regular, IR = Irregular). |
| **LandContour** | Categorical | Flatness of property (Lvl, HLS, Low, Bnk). |
| **Utilities** | Categorical | Utilities available (AllPub, NoSeWa, etc.). |
| **LotConfig** | Categorical | Lot configuration (Inside, Corner, CulDSac, etc.). |
| **LandSlope** | Categorical | Slope of property (Gtl, Mod, Sev). |
| **Neighborhood** | Categorical | Physical location within Ames city. |
| **Condition1** | Categorical | Proximity to main road/railroad. |
| **Condition2** | Categorical | Secondary proximity to road/railroad. |

---

##  Building & Style
| Feature | Type | Description |
|---------|------|-------------|
| **BldgType** | Categorical | Type of dwelling (1Fam, 2FmCon, Duplex, Twnhs). |
| **HouseStyle** | Categorical | Dwelling style (1Story, 2Story, Split, etc.). |
| **OverallQual** | Ordinal | Overall material and finish quality (1–10). |
| **OverallCond** | Ordinal | Overall condition rating (1–10). |
| **YearBuilt** | Integer | Original construction date. |
| **YearRemodAdd** | Integer | Remodel date (same as YearBuilt if never remodeled). |

---

##  Roof & Exterior
| Feature | Type | Description |
|---------|------|-------------|
| **RoofStyle** | Categorical | Roof type (Gable, Hip, etc.). |
| **RoofMatl** | Categorical | Roof material. |
| **Exterior1st** | Categorical | Exterior covering (1st material). |
| **Exterior2nd** | Categorical | Exterior covering (2nd material). |
| **MasVnrType** | Categorical | Masonry veneer type (BrkFace, Stone, None). |
| **MasVnrArea** | Numeric | Masonry veneer area in sq. ft. |
| **ExterQual** | Ordinal | Exterior quality (Ex, Gd, TA, Fa, Po). |
| **ExterCond** | Ordinal | Exterior condition. |

---

##  Foundation & Basement
| Feature | Type | Description |
|---------|------|-------------|
| **Foundation** | Categorical | Foundation type (PConc, CBlock, BrkTil, etc.). |
| **BsmtQual** | Ordinal | Basement height (Ex, Gd, TA, Fa, NA). |
| **BsmtCond** | Ordinal | Basement condition. |
| **BsmtExposure** | Categorical | Walkout or garden level basement walls. |
| **BsmtFinType1** | Categorical | Rating of finished basement area (GLQ, ALQ, etc.). |
| **BsmtFinSF1** | Numeric | Type 1 finished sq. ft. |
| **BsmtFinType2** | Categorical | Rating of 2nd finished area (if present). |
| **BsmtFinSF2** | Numeric | Type 2 finished sq. ft. |
| **BsmtUnfSF** | Numeric | Unfinished basement sq. ft. |
| **TotalBsmtSF** | Numeric | Total basement area. |

---

##  Heating, Cooling & Utilities
| Feature | Type | Description |
|---------|------|-------------|
| **Heating** | Categorical | Heating type (GasA, GasW, Grav, Wall, etc.). |
| **HeatingQC** | Ordinal | Heating quality & condition. |
| **CentralAir** | Categorical | Central air conditioning (Y/N). |
| **Electrical** | Categorical | Electrical system (SBrkr, FuseA, etc.). |

---

##  Interior (Rooms & Living Areas)
| Feature | Type | Description |
|---------|------|-------------|
| **1stFlrSF** | Numeric | First floor sq. ft. |
| **2ndFlrSF** | Numeric | Second floor sq. ft. |
| **LowQualFinSF** | Numeric | Low quality finished sq. ft. |
| **GrLivArea** | Numeric | Above ground living area sq. ft. |
| **BsmtFullBath** | Numeric | Basement full bathrooms. |
| **BsmtHalfBath** | Numeric | Basement half bathrooms. |
| **FullBath** | Numeric | Full bathrooms above grade. |
| **HalfBath** | Numeric | Half bathrooms above grade. |
| **BedroomAbvGr** | Numeric | Bedrooms above grade. |
| **KitchenAbvGr** | Numeric | Kitchens above grade. |
| **KitchenQual** | Ordinal | Kitchen quality. |
| **TotRmsAbvGrd** | Numeric | Total rooms above grade. |
| **Functional** | Categorical | Home functionality rating. |
| **Fireplaces** | Numeric | Number of fireplaces. |
| **FireplaceQu** | Ordinal | Fireplace quality. |

---

##  Garage & Parking
| Feature | Type | Description |
|---------|------|-------------|
| **GarageType** | Categorical | Garage location (Attchd, Detchd, BuiltIn, etc.). |
| **GarageYrBlt** | Numeric | Year garage built. |
| **GarageFinish** | Categorical | Garage interior finish. |
| **GarageCars** | Numeric | Garage size (car capacity). |
| **GarageArea** | Numeric | Garage size (sq. ft.). |
| **GarageQual** | Ordinal | Garage quality. |
| **GarageCond** | Ordinal | Garage condition. |
| **PavedDrive** | Categorical | Paved driveway (Y/N/P). |

---

##  Outdoor Features
| Feature | Type | Description |
|---------|------|-------------|
| **WoodDeckSF** | Numeric | Wood deck area (sq. ft.). |
| **OpenPorchSF** | Numeric | Open porch area (sq. ft.). |
| **EnclosedPorch** | Numeric | Enclosed porch area (sq. ft.). |
| **3SsnPorch** | Numeric | Three-season porch area (sq. ft.). |
| **ScreenPorch** | Numeric | Screen porch area (sq. ft.). |
| **PoolArea** | Numeric | Pool area (sq. ft.). |
| **PoolQC** | Ordinal | Pool quality. |
| **Fence** | Categorical | Fence quality (GdPrv, MnPrv, GdWo, etc.). |
| **MiscFeature** | Categorical | Miscellaneous features (Shed, TenC, etc.). |
| **MiscVal** | Numeric | Value of misc. feature. |

---

##  Sale Information
| Feature | Type | Description |
|---------|------|-------------|
| **MoSold** | Integer | Month sold. |
| **YrSold** | Integer | Year sold. |
| **SaleType** | Categorical | Sale type (WD, New, COD, etc.). |
| **SaleCondition** | Categorical | Condition of sale (Normal, Abnorml, Family, etc.). |
| **SalePrice** | Numeric | Target variable – Sale price in USD. |

---
  
