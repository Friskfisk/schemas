# Journal Schema

```txt
https://poseidat.org/schema/core/journal.json
```

A trip journal


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                       |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | ---------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [journal.json](schemas/core/journal.json "open original schema") |

## Journal Type

`object` ([Journal](journal.md))

# Journal Properties

| Property                  | Type     | Required | Nullable       | Defined by                                                                                                              |
| :------------------------ | -------- | -------- | -------------- | :---------------------------------------------------------------------------------------------------------------------- |
| [journal_id](#journal_id) | `string` | Required | cannot be null | [Journal](journal-properties-journal_id.md "https&#x3A;//poseidat.org/schema/core/journal.json#/properties/journal_id") |
| [vessel](#vessel)         | `object` | Required | cannot be null | [Journal](journal-properties-vessel.md "https&#x3A;//poseidat.org/schema/core/vessel.json#/properties/vessel")          |

### Cooper: We need to put some gear type classification as many vessels switch gear types. It seems to me this is the initial place where gear type should go, although we may eventually want to put in a seperate schema that is referenced in journal for tracking mesh size, spread, ground gear, etc?

## journal_id

The unique identifier for the journal (UUID v4)


`journal_id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Journal](journal-properties-journal_id.md "https&#x3A;//poseidat.org/schema/core/journal.json#/properties/journal_id")

### journal_id Type

`string`

### journal_id Constraints

**UUID**: the string must be a UUID, according to [RFC 4122](https://tools.ietf.org/html/rfc4122 "check the specification")

## vessel

The vessel information


`vessel`

-   is required
-   Type: `object` ([Vessel](journal-properties-vessel.md))
-   cannot be null
-   defined in: [Journal](journal-properties-vessel.md "https&#x3A;//poseidat.org/schema/core/vessel.json#/properties/vessel")

### vessel Type

`object` ([Vessel](journal-properties-vessel.md))
