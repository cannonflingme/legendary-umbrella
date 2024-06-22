{
    "env": {
        "node": true,
        "browser": true,
        "es2021": true
    },
    "extends": [
        // "eslint:recommended",
        "prettier"
    ],
    "parserOptions": {
        "sourceType": "module",
        "ecmaVersion": 2022
    },
    "rules": {
        // Possible Errors (overrides from recommended set)

        // "no-extra-parens": "error",
        "no-unexpected-multiline": "error",

        // All JSDoc comments must be valid
        
        "valid-jsdoc": [ "error", {
            "requireReturn": true,
            "requireReturnDescription": true,
            "requireParamDescription": true,
            "prefer": {
                "return": "returns"
            }
        }],

        // Best Practices

        // Allowed a getter without setter, but all setters require getters

        "accessor-pairs": [ "error", {
            "getWithoutSet": false,
            "setWithoutGet": true
        }],
        "block-scoped-var": "warn",
        "consistent-return": "error",
        "curly": "error",
        // "default-case": "warn",

        // the dot goes with the property when doing multiline

        // "dot-location": [ "warn", "property" ],
        // "dot-notation": "warn",
        // "eqeqeq": [ "error", "smart" ],
        // "guard-for-in": "warn",
        "no-alert": "error",
        "no-caller": "error",
        // "no-case-declarations": "warn",
        // "no-div-regex": "warn",
        // "no-else-return": "warn",
        // "no-empty-label": "warn",
        // "no-empty-pattern": "warn",
        // "no-eq-null": "warn",
        // "no-eval": "error",
        // "no-extend-native": "error",
        // "no-extra-bind": "warn",
        // "no-floating-decimal": "warn",
        // "no-implicit-coercion": [ "warn", {
        //     "boolean": true,
        //     "number": true,
        //     "string": true
        // }],
        // "no-implied-eval": "error",
        // "no-invalid-this": "error",
        // "no-iterator": "error",
        // "no-labels": "warn",
        // "no-lone-blocks": "warn",
        // "no-loop-func": "error",
        // "no-magic-numbers": "warn",
        // "no-multi-spaces": "error",
        // "no-multi-str": "warn",
        // "no-native-reassign": "error",
        // "no-new-func": "error",
        // "no-new-wrappers": "error",
        // "no-new": "error",
        // "no-octal-escape": "error",
        // "no-param-reassign": "error",
        // "no-process-env": "warn",
        // "no-proto": "error",
        // "no-redeclare": "error",
        // "no-return-assign": "error",
        // "no-script-url": "error",
        // "no-self-compare": "error",
        // "no-throw-literal": "error",
        // "no-unused-expressions": "error",
        // "no-useless-call": "error",
        // "no-useless-concat": "error",
        // "no-void": "warn",

        // Produce warnings when something is commented as TODO or FIXME

        "no-warning-comments": [ "warn", {
            "terms": [ "TODO", "FIXME" ],
            "location": "start"
        }],
        "no-with": "warn",
        "radix": "warn",
        // "vars-on-top": "error",

        // Enforces the style of wrapped functions
        // "wrap-iife": [ "error", "outside" ],
        // "yoda": "error",

        // Strict Mode - for ES6, never use strict.
        // "strict": [ "error", "never" ],

        // Variables

        // "init-declarations": [ "error", "always" ],
        // "no-catch-shadow": "warn",
        "no-delete-var": "error",
        // "no-label-var": "error",
        // "no-shadow-restricted-names": "error",
        // "no-shadow": "warn",

        // We require all vars to be initialized (see init-declarations)
        // If we NEED a var to be initialized to undefined, it needs to be explicit

        "no-undef-init": "off",
        "no-undef": "error",
        "no-undefined": "off",
        "no-unused-vars": "warn",

        // Disallow hoisting - let & const don't allow hoisting anyhow

        "no-use-before-define": "error",

        // Node.js and CommonJS

        // "callback-return": [ "warn", [ "callback", "next" ]],
        // "global-require": "error",
        // "handle-callback-err": "warn",
        // "no-mixed-requires": "warn",
        // "no-new-require": "error",

        // Use path.concat instead

        // "no-path-concat": "error",
        // "no-process-exit": "error",
        // "no-restricted-modules": "off",
        // "no-sync": "warn",

        // ECMAScript 6 support

        // "arrow-body-style": [ "error", "always" ],
        // "arrow-parens": [ "error", "always" ],
        // "arrow-spacing": [ "error", { "before": true, "after": true }],
        "constructor-super": "error",
        // "generator-star-spacing": [ "error", "before" ],
        // "no-arrow-condition": "error",
        "no-class-assign": "error",
        "no-const-assign": "error",
        "no-dupe-class-members": "error",
        "no-this-before-super": "error",
        // "no-var": "warn",
        "object-shorthand": [ "warn" ],
        // "prefer-arrow-callback": "warn",
        // "prefer-spread": "warn",
        // "prefer-template": "warn",
        // "require-yield": "error",

        // Stylistic - everything here is a warning because of style.

        // "array-bracket-spacing": [ "warn", "always" ],
        // "block-spacing": [ "warn", "always" ],
        // "brace-style": [ "warn", "1tbs", { "allowSingleLine": false } ],
        // "camelcase": "warn",
        // "comma-spacing": [ "warn", { "before": false, "after": true } ],
        // "comma-style": [ "warn", "last" ],
        // "computed-property-spacing": [ "warn", "never" ],
        // "consistent-this": [ "warn", "self" ],
        // "eol-last": "warn",
        // "func-names": "warn",
        // "func-style": [ "warn", "declaration" ],
        // "id-length": [ "warn", { "min": 2, "max": 32 } ],
        // "indent": [ "warn", 4 ],
        // "jsx-quotes": [ "warn", "prefer-double" ],
        // "linebreak-style": [ "warn", "unix" ],
        // "lines-around-comment": [ "warn", { "beforeBlockComment": true } ],
        // "max-depth": [ "warn", 8 ],
        // "max-len": [ "warn", 132 ],
        // "max-nested-callbacks": [ "warn", 8 ],
        // "max-params": [ "warn", 8 ],
        // "new-cap": "warn",
        // "new-parens": "warn",
        // "no-array-constructor": "warn",
        // "no-bitwise": "off",
        // "no-continue": "off",
        // "no-inline-comments": "off",
        // "no-lonely-if": "warn",
        "no-mixed-spaces-and-tabs": "warn",
        "no-multiple-empty-lines": "warn",
        "no-negated-condition": "warn",
        // "no-nested-ternary": "warn",
        // "no-new-object": "warn",
        // "no-plusplus": "off",
        // "no-spaced-func": "warn",
        // "no-ternary": "off",
        // "no-trailing-spaces": "warn",
        // "no-underscore-dangle": "warn",
        "no-unneeded-ternary": "warn",
        // "object-curly-spacing": [ "warn", "always" ],
        // "one-var": "off",
        // "operator-assignment": [ "warn", "never" ],
        // "operator-linebreak": [ "warn", "after" ],
        // "padded-blocks": [ "warn", "never" ],
        // "quote-props": [ "warn", "consistent-as-needed" ],
        // "quotes": [ "warn", "single" ],
        "require-jsdoc": [ "warn", {
            "require": {
                "FunctionDeclaration": true,
                "MethodDefinition": true,
                "ClassDeclaration": false
            }
        }],
        // "semi-spacing": [ "warn", { "before": false, "after": true }],
        // "semi": [ "error", "always" ],
        // "sort-vars": "off",
        "keyword-spacing": ["error", { "before": true, "after": true }]
        // "space-before-blocks": [ "warn", "always" ],
        // "space-before-function-paren": [ "warn", "never" ],
        // "space-in-parens": [ "warn", "never" ],
        // "space-infix-ops": [ "warn", { "int32Hint": true } ],
        // "space-return-throw-case": "error",
        // "space-unary-ops": "error",
        // "spaced-comment": [ "warn", "always" ],
        // "wrap-regex": "warn"
    }
}
