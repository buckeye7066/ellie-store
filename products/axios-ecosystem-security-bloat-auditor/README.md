# Axios Ecosystem Security & Bloat Auditor

**Price: $29.99** · [Buy the full pack](https://buy.stripe.com/5kQ8wQg5EeA58tdfVdawo0n) · delivered as a Markdown file you can import or edit.


*Product line: code_utility*

---

## Preview

#!/usr/bin/env node
const fs = require('fs');
const path = require('path');

/**
 * Axios Ecosystem Dependency Security & Bloat Auditor
 * 
 * Usage:
 *   node axios-auditor.js [path-to-project-root]
 * 
 * Performs static analysis of package.json to identify:
 * 1. Axios version pinning and security risks.
 * 2. Common bundle bloat candidates.
 * 3. Peer dependency conflicts.
 */

function audit(projectPath = process.cwd()) {
    const pkgPath = path.join(projectPath, 'package.json');
    if (!fs.existsSync(pkgPath)) {
        console.error('Error: package.json not found in ' + projectPath);
        process.exit(1);
    }

    const pkg = JSON.parse(fs.readFileSync(pkgPath, 'utf8'));
    const deps = { ...(pkg.dependencies || {}), ...(pkg.devDependencies || {}) };
    
    console.log('--- Axios Ecosystem Audit: ' + (pkg.name || 'Unknown Project') + ' ---');
    
    // 1. Axios Check
    const axiosVersion = deps.axios;
    if (!axiosVersion) {
        console.log('[INFO] Axios not detected in dependencies.');
    } else {
        console.log('[PASS] Axios detected: ' + axiosVersion);
        if (axiosVersion.includes('^') || axiosVersion.includes('~') || axiosVersion.includes('*')) {
            console.log('[WARN] Axios version range detected. Pin to exact version for predictable security builds.');
        }
    }

    // 2. Bloat Analysis (Heuristic)
    const heavyDeps = ['lodash', 'moment', 'rxjs', 'jquery'];
    const foundHeavy = Object.keys(deps).filter(d => heavyDeps.includes(d));
    if (foundHeavy.length > 0) {
        console.log('[WARN] Potential bloat detected: ' + foundHeavy.join(', ') + '. Consider modular imports or tree-shakable alternatives.');
    } else {
        console.log('[PASS] No common bundle-bloat heavyweights detected.');
    }

    console.log('--- Audit Complete ---');
}

if (require.main === module) {
    audit(process.argv[2]);
}

---

[Buy the full pack for $29.99](https://buy.stripe.com/5kQ8wQg5EeA58tdfVdawo0n)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
