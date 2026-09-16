# Portfolio Data Schema

This schema defines the minimum structured information the agent should preserve per asset so future analysis can be automated.

## Record keys

```yaml
asset_id: string
created_at: date
submitted_at: date|null
published_at: date|null
concept_family: string
sub_niche: string
buyer_use_cases: [string]
seasonality: evergreen|seasonal|event|emerging
format: portrait|landscape|square|other
aspect_ratio: string
portfolio_cluster: string
research:
  date: date
  official_adobe_sources: [url]
  external_sources: [url]
  demand_signal: string
  signal_strength: anecdotal|weak|preliminary|useful|strong
  saturation: low|medium|high|unknown
  differentiation: string
production:
  tool: string
  model_version: string|null
  prompt_version: string
  attempt: integer
technical:
  width_px: integer
  height_px: integer
  megapixels: number
  format: JPEG
  color_space: sRGB
  file_size_mb: number
  qc_100_percent: pass|fail
compliance:
  generative_ai_label: yes|no|unknown
  fictional_people_property_label: yes|no|n_a|unknown
  releases: none|attached|review|unknown
  ip_legal: pass|fail|hold
  license: pass|fail|hold
  similarity: pass|fail|hold
submission:
  status: not_submitted|submitted|accepted|refused|unknown
  refusal_category: string|null
  refusal_text: string|null
performance:
  observation_start: date|null
  observation_end: date|null
  days_live: integer|null
  impressions: number|null
  downloads: number|null
  revenue: number|null
  favorites: number|null
learning:
  hypothesis_id: string|null
  lesson: string|null
  evidence_strength: anecdote|weak|preliminary|useful|strong|unknown
```

## Missing data policy

`null` means unavailable. `0` means observed zero. Never replace unavailable metrics with zero.

## Privacy policy

Do not store credentials, session cookies, API keys, payment information or unrelated personal data.
