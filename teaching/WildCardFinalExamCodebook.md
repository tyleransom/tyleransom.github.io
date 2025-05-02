# College Admissions Dataset Codebook

This codebook describes the simulated college admissions dataset generated for analysis. The data simulates college applications across different demographic groups with various academic credentials and institutional ratings.

## Procedural Variables

| Variable | Description | Type | Values |
|----------|-------------|------|--------|
| applicant_id | Unique identifier for each applicant | Integer | 1 to 155,356 |
| year | Application year | Integer | 2014 to 2019 |
| completed_app | Whether application was completed | Binary | 0 = incomplete, 1 = complete |

## Outcome Variable

| Variable | Description | Type | Values |
|----------|-------------|------|--------|
| admit | Admission decision | Binary | 0 = rejected, 1 = admitted, missing = incomplete application |

## Demographic Variables

| Variable | Description | Type | Values |
|----------|-------------|------|--------|
| group | Demographic group category | String | A, B, C, D, E (labels for different demographic groups) |
| female | Gender indicator | Binary | 0 = male, 1 = female |
| disadvantaged | Socioeconomic status indicator | Binary | 0 = not socioeconomically disadvantaged, 1 = socioeconomically disadvantaged |
| first_generation | First-generation college student status | Binary | 0 = not first-generation, 1 = first-generation |
| early_decision | Applied through early decision | Binary | 0 = regular decision, 1 = early decision |
| waiver | Received application fee waiver | Binary | 0 = did not receive waiver, 1 = received waiver |
| applied_financial_aid | Applied for financial aid | Binary | 0 = did not apply, 1 = applied |
| intended_major | Intended field of study | String | "Humanities", "Biology", "Physical Sciences", "Engineering", "Mathematics", "Computer Science", "Unspecified" |

## Academic Preparation Variables

| Variable | Description | Type | Values |
|----------|-------------|------|--------|
| sat_math | SAT Math score (standardized) | Float | Standardized scores (mean ≈ 0, SD ≈ 1) |
| sat_verbal | SAT Verbal score (standardized) | Float | Standardized scores (mean ≈ 0, SD ≈ 1) |
| hs_gpa | High school GPA (standardized) | Float | Standardized scores (mean ≈ 0, SD ≈ 1) |
| acad_index | Academic index (composite measure, standardized) | Float | Standardized scores (mean ≈ 0, SD ≈ 1) |
| ap_tests | Number of AP tests taken | Integer | 0 to 20 |
| ap_score | Average AP test score | Float | 1 to 5 (missing if ap_tests = 0) |

## Subjective Rating Variables

All ratings are on a 1-4 scale where 1 is the highest rating and 4 is the lowest rating. All are missing if completed_app = 0.

| Variable | Description | Type | Values |
|----------|-------------|------|--------|
| academic_rating | Academic preparation rating | Ordinal | 1 (highest) to 4 (lowest) |
| extracurricular_rating | Extracurricular activities rating | Ordinal | 1 (highest) to 4 (lowest) |
| athletic_rating | Athletic abilities rating | Ordinal | 1 (highest) to 4 (lowest) |
| teacher1_rating | First high school teacher recommendation rating | Ordinal | 1 (highest) to 4 (lowest) |
| teacher2_rating | Second high school teacher recommendation rating | Ordinal | 1 (highest) to 4 (lowest) |
| counselor_rating | School counselor recommendation rating | Ordinal | 1 (highest) to 4 (lowest) |
| personal_rating | Personal qualities rating (assigned by admissions officer) | Ordinal | 1 (highest) to 4 (lowest) |
| alumnipers_rating | Personal qualities rating (assigned by alumni interviewer) | Ordinal | 1 (highest) to 4 (lowest) |
