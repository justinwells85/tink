# Database Schema

## Overview

The system uses a structured AWS-hosted database for RAG and analytics.

## Core Tables

### workflows
- `id` (PK)
- `name`
- `description`
- `trigger_phrases` (array or join to separate table)
- `created_at`
- `updated_at`

### workflow_steps
- `id` (PK)
- `workflow_id` (FK)
- `step_number`
- `instruction`
- `expected_input_type` (enum: YES_NO, TEXT, CHECKBOX, FILE_UPLOAD)

### session_logs
- `id` (PK)
- `user_id`
- `workflow_id`
- `start_time`
- `end_time`
- `status` (enum: COMPLETED, ABANDONED, ESCALATED)

### step_logs
- `id` (PK)
- `session_id` (FK)
- `step_id` (FK)
- `completed_at`
- `response_value`

