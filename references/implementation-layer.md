# Engineering Implementation Layer

Use this layer when the plan is meant to be executed by Codex, another agent, or a developer.

## Required Header

Every executable implementation plan must include:

```markdown
> **For agentic workers:** REQUIRED: Use superpowers:subagent-driven-development if available, or superpowers:executing-plans to implement this plan. Steps use checkbox syntax for tracking.
```

## File Structure First

Before tasks, map exact files:

```markdown
## 文件结构与模块边界

- Create: `src/features/foo/model.ts`
- Modify: `src/features/foo/service.ts`
- Modify: `src/routes/foo.tsx`
- Test: `src/features/foo/foo.test.ts`

### 模块边界

- `model.ts` 只负责类型、schema 和解析。
- `service.ts` 负责业务逻辑和外部调用。
- UI 组件只处理展示和用户交互，不直接处理数据转换。
```

## Task Granularity

Each step should be one small action, usually 2-5 minutes:

- Write failing test.
- Run test to verify it fails.
- Implement minimal code.
- Run test to verify it passes.
- Commit.

Avoid broad steps like "implement validation" or "add tests". Include code, commands, and expected results.

## Task Template

````markdown
### Task N: [Component Name]

**Files:**
- Create: `exact/path/to/file.ts`
- Modify: `exact/path/to/existing.ts`
- Test: `exact/path/to/test.ts`

- [ ] **Step 1: Write the failing test**

```ts
it("validates the specific behavior", () => {
  const result = functionUnderTest(input);
  expect(result).toEqual(expected);
});
```

- [ ] **Step 2: Run test to verify it fails**

Run: `npm test -- exact/path/to/test.ts`
Expected: FAIL with `[specific missing behavior]`

- [ ] **Step 3: Write minimal implementation**

```ts
export function functionUnderTest(input: Input): Output {
  return expected;
}
```

- [ ] **Step 4: Run test to verify it passes**

Run: `npm test -- exact/path/to/test.ts`
Expected: PASS

- [ ] **Step 5: Commit**

```bash
git add exact/path/to/file.ts exact/path/to/test.ts
git commit -m "feat: add specific behavior"
```
````

## Testing Layer

For every plan, specify:

- Unit tests for pure logic and parsing.
- Integration tests for service boundaries.
- E2E or smoke tests for critical user flows.
- Manual checks for UI/UX or migration behavior when automation is insufficient.
- Expected output for each command.

## Acceptance Layer

Use official-plan style indicators plus engineering checks:

```markdown
### 约束性目标

- `npm test -- src/features/foo` passes.
- Existing smoke tests pass.
- API contract remains backward compatible.
- No new high-severity lint/type errors.

### 预期性目标

- User task completion time decreases.
- Duplicate logic is reduced.
- Future features can reuse the new service entry point.
```

## Commit and Review

Prefer frequent commits at meaningful boundaries:

- One commit per self-contained task.
- Commit after tests pass.
- Include review points for risky changes: data migration, security, public API, billing/payment, auth, deletion, permissions, or rollout.

