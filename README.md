# JobFit Radar
## Job research with structured AI-assisted review

JobFit Radar brings opportunities into a single review workflow, filters unsuitable listings and uses an LLM to explain alignment with a candidate's background. It is a personal application designed to make research more organized and its reasoning easier to inspect.

**Context:** Individually developed personal application. It is not a commercial recruiting service or an automated hiring decision system.

## Who it is for and what it solves

Job seekers reviewing listings across sources need a way to organize opportunities, reduce duplicate review and understand why a role may or may not fit. JobFit Radar combines data processing with structured explanations rather than presenting an unexplained score alone.

## How it works

1. Collect opportunities through configured source integrations.
2. Normalize and deduplicate collected listings, then apply initial filters.
3. Analyze selected listings against candidate context using OpenAI.
4. Validate structured output and retain results with scan status.
5. Incorporate prior feedback into later prompt context for continued review.

## My contribution

I built the application individually, connecting ingestion, scan orchestration, filtering, structured AI analysis and review feedback. I also added error-path tests for malformed model output, invalid score bounds and missing configuration.

## Implementation and evidence

Next.js, TypeScript, Supabase, OpenAI, Zod and Vitest. Current source confirms actual model calls and schema validation. Test source covers structured-output and configuration error handling. Feedback is supplied as prompt context; it is not model fine-tuning.

## Access and boundaries

Source and personal information remain private. No verified public demo is currently linked. A demonstration should use fictional candidate details and sample listings, not private resumes, inbox messages or application histories.

Fit scores are qualitative aids, not calibrated hiring probabilities. Model explanations support, rather than replace, human review.
