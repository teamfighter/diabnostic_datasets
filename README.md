# Diabnostic Datasets

Open anonymized datasets from [Diabnostic](https://diabnostic.ru) — a pet diabetes monitoring platform.

## 📂 Datasets

### glucose/

**glucose_records.csv** — 6 773 glucose measurements from 117 diabetic pets (110 cats, 7 dogs) collected over 5 months (November 2025 – March 2026).

| Column | Type | Description |
|--------|------|-------------|
| `pet_id` | int | Anonymized pet identifier (1–117) |
| `species` | str | `cat` or `dog` |
| `sex` | str | `male` or `female` |
| `age_years` | float | Pet age in years |
| `weight_kg` | float | Pet weight in kilograms |
| `sterilized` | str | `yes`, `no`, or `unknown` |
| `insulin_group` | str | Insulin active ingredient (e.g., `Detemir`, `Glargine_U100`) |
| `glucose_mmol` | float | Blood glucose level (mmol/L) |
| `insulin_dose_u` | float | Insulin dose (units) |
| `date` | date | Measurement date (YYYY-MM-DD) |
| `time` | time | Measurement time (HH:MM) |

#### Key statistics

- **Median glucose:** 14.5 mmol/L (IQR: 7.9–19.7)
- **Target range (4–10 mmol/L):** 28.8% of all readings
- **Hypoglycemia (< 3.5):** 4.9% of readings
- **Records per pet:** median 16, max 340

#### Data collection

All measurements are manually entered by pet owners using home glucometers. Basic validation is applied (glucose: 0.1–50 mmol/L, dose: 0–100 U), but accuracy may vary due to different devices and measurement conditions.

## 🔒 Anonymization

- Pet IDs are replaced with sequential numbers (no mapping to real IDs)
- Pet names are **not included**
- Owner/user information is **not included**
- No access codes, notes, or other identifying information

## 📄 License

This dataset is licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/).

You are free to:
- **Share** — copy and redistribute the material
- **Adapt** — remix, transform, and build upon the material

Under the following terms:
- **Attribution** — credit Diabnostic as the source
- **NonCommercial** — not for commercial purposes

For commercial use, please contact the author.

## 📖 Related

- **Platform:** [diabnostic.ru](https://diabnostic.ru)
- **Habr article:** *(coming soon)*

## 🤝 Contributing

If you find interesting patterns in the data or want to collaborate on analysis — open an issue or reach out!