# workspace

## 신규 서비스 기획 에이전트 팀

`.claude/agents/`에 신규 서비스 기획을 위한 서브에이전트 4종이 정의되어 있습니다. 아래 순서로 이어지는 파이프라인이며, 각 단계 결과물은 `docs/planning/`에 저장됩니다.

1. `market-researcher` — 시장/경쟁사/타겟 유저 조사 → `docs/planning/market-research.md`
2. `biz-model-planner` — 수익모델/가격 정책/사업성 검토 → `docs/planning/business-model.md`
3. `prd-writer` — PRD(기능 요구사항) 작성 → `docs/planning/prd.md`
4. `ux-flow-designer` — 유저 플로우/화면 구조 설계 → `docs/planning/ux-flow.md`

Claude Code에서 `Agent` 도구로 각 에이전트를 이름으로 호출하거나, 관련 요청("시장 조사해줘", "PRD 작성해줘" 등)을 하면 자동으로 매칭되는 에이전트가 사용됩니다.