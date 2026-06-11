# Hướng Dẫn Nộp Bài — Day 11

## Bạn cần nộp 2 file chính

| File | Mô tả |
|------|--------|
| `notebooks/assignment11_defense_pipeline.ipynb` | **Assignment 11** — pipeline 6 lớp + 4 test suites (60 điểm) |
| `submissions/bao_cao_ca_nhan_assignment11.md` | **Báo cáo cá nhân** tiếng Việt (40 điểm) → export PDF nếu giảng viên yêu cầu |

**Tuỳ chọn (lab):** `notebooks/lab11_guardrails_hitl.ipynb` — đã hoàn thành 13 TODO.

---

## Trước khi nộp — checklist

- [ ] Điền **tên + MSSV** vào đầu notebook và báo cáo
- [ ] Chạy **Run All** notebook assignment → có output Test 1–4
- [ ] File `security_audit.json` được tạo (cell cuối)
- [ ] **Không** commit `GOOGLE_API_KEY` vào git
- [ ] Export báo cáo `.md` → `.pdf` nếu cần

---

## Chạy local nhanh

```bash
cd Day-11-Guardrails-HITL-Responsible-AI
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt

export GOOGLE_API_KEY="your-key"
export NEMOGUARDRAILS_LLM_FRAMEWORK=langchain
export GOOGLE_GENAI_USE_VERTEXAI=0

jupyter notebook notebooks/assignment11_defense_pipeline.ipynb
```

**Lưu ý:** Cần internet + API key Gemini. Chạy full notebook mất ~5–10 phút.

---

## Cấu trúc điểm

| Phần | Điểm | File |
|------|------|------|
| Notebook pipeline | 60 | `assignment11_defense_pipeline.ipynb` |
| Báo cáo cá nhân | 40 | `bao_cao_ca_nhan_assignment11.md` |
| Bonus lớp thứ 6 | +10 | Cell Bonus trong notebook (language detection) |
