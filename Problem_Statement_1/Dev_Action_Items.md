# Development Action Items

## List for Discussion with Dev Team:

### Backend:
- Integrate with a vulnerability scanner (e.g., Trivy, Clair).
- Build REST API endpoints:
  - GET /images: List all images with vulnerability counts.
  - GET /images/:id: Get detailed findings for an image.
  - POST /scan: Trigger scan for an image.
- Implement pagination for large datasets.

### Frontend:
- Use React/Vue for the dashboard.
- Implement table with sorting/filtering (e.g., Material-UI DataGrid).
- Add search functionality with debounce for performance.

### DevOps:
- Set up CI/CD for frontend/backend deployment.
- Deploy to Kubernetes with autoscaling for high traffic.

### Security:
- Implement OAuth for user authentication.
- Use HTTPS for API calls.