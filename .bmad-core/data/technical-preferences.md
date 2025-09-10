<!-- Powered by BMAD™ Core -->

# User-Defined Preferred Patterns and Preferences

## Use these technologies: 

Always prefer the latest versions of these technologies. Use at least the version given. Always use the latest features of these libraries and frameworks. Avoid using deprecated features and syntax.

### Next.js 15+

Read https://nextjs.org/blog/next-15 and use the latest features. Do not use deprecated features, such as getInitialProps.

### React 19+

Read https://react.dev/blog/2024/12/05/react-19 and use the latest features. Do not use deprecated features, such as forwardRef.

### Convex

Use Convex as the backend.

For presence, use these patterns: https://stack.convex.dev/presence-with-convex

For Convex functions, use these patterns: https://stack.convex.dev/custom-functions

Instead of creating interfaces for use across the application, use the Convex type system as shown here: https://stack.convex.dev/end-to-end-ts

For authorization, use these patterns: https://stack.convex.dev/authorization

Use Zod with TypeScript for Server-side Validation and End-to-End Types as shown here: https://stack.convex.dev/typescript-zod-function-validation. We will be using Zod 4, which is a little bit different from Zod 3, which is used in the example above. But, use the patterns from the article above.

### Convex Auth
### TailwindCSS 4+
### Licide
### shadcn/ui

Use the shadcn MCP server to discover and learn how to use shadcn components. Also prefer to use tweakcn for theming. The application must support both light mode and dark mode.

### shadcn blocks

Use the shadcn MCP server to discover and learn how to use shadcn blocks.

### resend (for outgoing email)
### Playwright 1.55+
### Vitest 3.2+
### Storybook 9+

Create stories for all components.

### Zod 4+

Read https://zod.dev/v4 and use the latest features. Do not use deprecated features or syntax. On the client, use Zod Mini where possible to reduce bundle size.

### XState 5+

Use XState for multistep forms.

### React Hook Form 7.62.0+

### gpt--oss-20b

For development, use the free version of the GPT model.

### GPT-5

For production, use the paid version of the GPT model.

### mapbox

## Patterns

### Modular Monolith

For speed, this will initially be a modular monolithic application. We will migrate to microservices later.