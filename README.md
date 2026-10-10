# Project M

A reusable Codex skill for turning personal records into evidence-based content topics.

## Contents

- `skills/personal-data-topics/`: the **个人资料选题研究** skill, with movie-specific research guidance and entry points for reading, running, travel, museums, football, and cross-domain topics.
- `topics/topic-library.md`: 32 research directions to test against a user's own records.

This public edition contains workflow instructions and topic seeds. Personal exports, reviews, ratings, machine paths, and generated media are not included.

## Install

Copy `skills/personal-data-topics` into `$CODEX_HOME/skills`, or `~/.codex/skills` when `CODEX_HOME` is unset. Keep the directory name `personal-data-topics`.

Example invocation:

> 使用 $personal-data-topics，从我的豆瓣数据中找5个电影史或演员相关选题，列出个人依据、比较方法、资料缺口和推荐顺序。

Provide the location of your own records and topic library. The skill has no custom runtime dependencies and does not include an automatic data collector. File analysis and web research use tools available in the current Codex environment.

## Scope

The workflow discovers candidates, checks evidence, designs comparisons, and maintains research cards. Movie-specific guidance distinguishes titles and IDs, viewing status and marking dates, personal and public ratings, box-office scopes, credits, story locations, and filming locations. Other domains have data requirements and interpretation rules; no external account connections are preconfigured.

Research and drafting do not authorize publishing or changing external content.

## Validation

Local checks covered frontmatter, reference files, invocation metadata, unfinished placeholders, and installation-copy integrity. The bundled `quick_validate.py` could not run in the authoring environment because PyYAML was unavailable. No claim of automated behavioral validation is made.
