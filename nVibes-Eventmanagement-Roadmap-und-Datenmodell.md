# nVibes Eventmanagement Roadmap & Datenmodell

**Dokumenttyp:** Produkt-, Architektur- und Entwicklungsleitfaden  
**Projekt:** nVibes  
**Bereich:** Vibe Feed, Event Creation, Event Details, My Events, Event Management  
**Version:** 1.0  
**Status:** Konzeption / Dev-Line für spätere Entwicklungsphase  
**Sprache:** Deutsch  

---

## 1. Executive Summary

Das Eventmanagement von nVibes soll nicht als klassisches, schweres Eventtool entstehen, sondern als natürliche Erweiterung des bestehenden Vibe-Systems.

Die Grundidee lautet:

> Ein User kann innerhalb weniger Sekunden einen Vibe posten, der gleichzeitig ein Event sein kann. Später kann dieses Event über „My Events“ in Ruhe erweitert, strukturiert und professionell verwaltet werden.

Damit entsteht ein bewusst zweistufiges beziehungsweise dreistufiges Produktmodell:

1. **Schnelles Erstellen im Vibe Feed**  
   Der User erstellt spontan ein Event mit wenigen Pflichtangaben.

2. **Ruhiges Bearbeiten in My Events**  
   Der User kann bestehende Events verwalten, Details ergänzen, Teilnehmer sehen und organisatorische Angaben pflegen.

3. **Erweiterbare Event-Level**  
   Ein Event startet als **Basis Event** und kann später auf **Advanced** oder **Professional** erweitert werden.

Das Ziel ist, die Spontaneität von nVibes zu erhalten und gleichzeitig langfristig eine professionelle Event-Infrastruktur aufzubauen.

---

## 2. Grundprinzip von nVibes Events

nVibes ist keine klassische Eventplattform. nVibes ist eine Social-Media-Plattform für echte Begegnungen im realen Leben.

Daher dürfen Events in nVibes nicht wie ein Verwaltungsformular wirken. Sie sollen sich anfühlen wie:

> „Ich habe Lust, etwas zu machen. Wer kommt mit?“

Ein Event ist deshalb zunächst ein sozialer Impuls. Erst später wird daraus bei Bedarf ein vollständig strukturiertes Event.

### 2.1 Zentrale Produktidee

Ein Event in nVibes ist ein spezieller Vibe.

Das bedeutet:

- Ein Event lebt im Feed.
- Ein Event kann kommentiert, geteilt und entdeckt werden.
- Ein Event kann spontan entstehen.
- Ein Event kann später erweitert werden.
- Ein Event bleibt sozial, nicht bürokratisch.

### 2.2 Kernentscheidung

Das System trennt bewusst zwischen:

| Ebene | Zweck |
|---|---|
| Vibe Feed | Spontane Sichtbarkeit und soziale Interaktion |
| Event Detail Layer | Strukturierte Informationen zum Event |
| My Events | Verwaltung, Bearbeitung und Ausbau durch den Host |

---

## 3. Produktlogik: Vom Vibe zum Event

### 3.1 Aktueller Gedanke

Beim Erstellen eines Posts kann der User sehr schnell einen Vibe veröffentlichen. Wenn dieser Vibe ein Event ist, werden nur minimale Daten benötigt:

- Eventname
- kurzer Text
- Datum
- Uhrzeit
- Ort oder Online-Angabe
- Bild
- Sichtbarkeit

Dadurch entsteht ein **Basis Event**, das sofort online ist.

### 3.2 Warum dieser Ansatz richtig ist

Klassische Eventplattformen scheitern oft daran, dass der User zu früh zu viele Informationen eingeben muss. Für nVibes wäre das falsch, weil die Plattform auf spontane reale Begegnungen ausgelegt ist.

Der richtige Flow ist:

> Erst veröffentlichen, dann verbessern.

Der User soll nicht am Anfang ein vollständiges Formular ausfüllen müssen. Er soll schnell einen sozialen Impuls setzen können.

---

## 4. Die drei Event-Level

nVibes Events sollten in drei klaren Stufen gedacht werden:

1. **Basis**
2. **Advanced**
3. **Professional**

Diese Level sind keine komplett unterschiedlichen Eventtypen. Sie sind Ausbaustufen desselben Eventmodells.

---

## 5. Level 1: Basis Event

### 5.1 Zielgruppe

Basis Events sind für spontane und einfache Treffen gedacht.

Beispiele:

- Kaffee trinken
- Spaziergang
- Lerngruppe
- kleiner Parktreff
- gemeinsames Mittagessen
- spontane Stadtaktivität
- „Wer hat Lust mitzukommen?“

### 5.2 Produktziel

Maximal geringe Hürde. Der User soll innerhalb weniger Sekunden posten können.

### 5.3 Pflichtfelder

Ein Basis Event benötigt nur:

| Feld | Beschreibung |
|---|---|
| title | Name des Events |
| description_short | kurzer Vibe-Text |
| start_datetime | Startdatum und Uhrzeit |
| location_label oder is_online | Ort oder Online-Markierung |
| cover_image | optionales oder empfohlenes Bild |
| visibility | Public, Private oder Invite Only |
| host_user_id | Ersteller / Host |

### 5.4 Optionale Felder

| Feld | Beschreibung |
|---|---|
| end_datetime | Ende des Events |
| max_attendees | Maximale Teilnehmerzahl |
| tags | Interessen und Suchbegriffe |
| category | grobe Einordnung |
| language | Sprache des Events |
| timezone | Zeitzone |

### 5.5 Feed-Darstellung

Im Feed darf ein Basis Event nicht überladen wirken. Sichtbar sein sollten:

- Bild
- Eventname
- Datum / Uhrzeit
- Ort
- kurzer Text
- Host
- Status wie „Hosting“
- Button „Details“
- Button „Teilnehmen“ oder „Join“

### 5.6 Was nicht in den Feed gehört

Folgende Dinge gehören nicht direkt in den Feed:

- lange Beschreibung
- vollständige Agenda
- Ticketlisten
- Speakerinformationen
- Sponsoren
- rechtliche Informationen
- Analytics
- komplexe Teilnehmerverwaltung

Diese Informationen gehören in den Detailbereich oder nach My Events.

---

## 6. Level 2: Advanced Event

### 6.1 Zielgruppe

Advanced Events sind für geplante Community-Events gedacht.

Beispiele:

- Community Meetup
- Workshop im kleinen Rahmen
- Uni-Gruppe
- Sportevent
- Spieleabend
- Nachbarschaftstreffen
- Vereinsähnliche Aktivitäten
- regelmäßige Treffen

### 6.2 Produktziel

Mehr Planung ermöglichen, ohne die User Experience schwer zu machen.

### 6.3 Zusätzliche Funktionen

Advanced Events können enthalten:

- lange Beschreibung
- genauer Treffpunkt
- Teilnehmerlimit
- Warteliste
- Teilnehmerverwaltung
- Check-in-Zeit
- Reminder
- einfache Agenda
- Kontaktinformationen
- Regeln / Hinweise
- Barrierefreiheit
- ÖPNV-Informationen
- Parkmöglichkeiten
- Wiederholungen

### 6.4 Typische Advanced-Felder

| Feld | Beschreibung |
|---|---|
| description_long | ausführliche Beschreibung |
| venue_id | strukturierter Veranstaltungsort |
| room_name | Raumname |
| floor | Etage |
| capacity | Kapazität |
| public_transport_info | Hinweise zum ÖPNV |
| accessibility_info | Barrierefreiheit |
| check_in_start | Beginn Check-in |
| doors_open | Einlasszeit |
| registration_open | Anmeldestart |
| registration_close | Anmeldeschluss |
| waitlist_enabled | Warteliste aktiv |
| recurrence_pattern | Wiederholungsmuster |
| organizer_contact_email | Kontaktadresse |
| organizer_contact_phone | Telefonnummer |

### 6.5 Advanced UX

In My Events sollte Advanced nicht als riesiger Formularblock erscheinen. Besser ist eine modulare Bearbeitung:

- Übersicht
- Beschreibung
- Zeitplanung
- Ort
- Teilnehmer
- Kommunikation
- Regeln & Sicherheit
- Wiederholung

---

## 7. Level 3: Professional Event

### 7.1 Zielgruppe

Professional Events sind für große, strukturierte oder kommerzielle Events gedacht.

Beispiele:

- Konferenzen
- Messen
- Festivals
- Konzerte
- öffentliche Workshops
- Creator Events
- bezahlte Events
- Firmenevents
- große Community-Veranstaltungen

### 7.2 Produktziel

nVibes soll langfristig auch professionelles Eventmanagement ermöglichen, ohne die spontane nVibes-DNA zu verlieren.

### 7.3 Professional-Funktionen

Professional Events können enthalten:

- Tickets und Preise
- Tickettypen
- Mengenbegrenzungen
- Verkaufslaufzeiten
- Zahlungsintegration
- Refund Policy
- Cancellation Policy
- Sessions
- Speaker
- Sponsoren
- Mediengalerie
- Dokumente
- Livestreams
- Online-Meeting-Daten
- Check-in-System
- Analytics
- Conversion Tracking
- Kalenderlinks
- Integrationen wie Zoom, YouTube, Stripe, PayPal
- rechtliche Angaben

### 7.4 Typische Professional-Module

| Modul | Zweck |
|---|---|
| Tickets | Verkauf, Kontingente, Preise |
| Sessions | Agenda / Programmplanung |
| Speakers | Referentenprofile |
| Sponsors | Sponsoring-Struktur |
| Media | Banner, Galerie, Dokumente |
| Legal | Terms, Privacy, Imprint, Waiver |
| Analytics | Views, Registrierungen, Umsatz |
| Integrations | Kalender, Payment, Streaming |

---

## 8. Upgrade-Flow: Event erweitern

### 8.1 Kernidee

Ein User startet mit Basis. Wenn das Event größer wird, kann er es erweitern.

Flow:

1. User erstellt Basis Event.
2. Event ist sofort live.
3. User öffnet My Events.
4. User klickt auf „Event erweitern“.
5. User wählt „Advanced aktivieren“ oder „Professional aktivieren“.
6. Zusätzliche Module werden freigeschaltet.
7. Vorhandene Daten bleiben erhalten.

### 8.2 Button-Bezeichnung

Empfohlene Bezeichnung:

> Event erweitern

Alternativen:

- Mehr Optionen freischalten
- Event ausbauen
- In Advanced umwandeln
- Professional aktivieren

### 8.3 UX-Texte

#### Advanced aktivieren

„Plane dein Event ausführlicher: Teilnehmerverwaltung, genaue Infos, Reminder, Warteliste und organisatorische Details.“

#### Professional aktivieren

„Nutze das volle Eventpaket: Tickets, Speaker, Sessions, Sponsoren, Analytics, rechtliche Infos und Integrationen.“

### 8.4 Technische Regel

Ein Upgrade darf keine bestehenden Daten löschen.

Das Event erhält lediglich:

- ein höheres `event_level`
- zusätzliche aktive Module
- zusätzliche Tabellenbeziehungen
- erweiterte UI-Bereiche in My Events

---

## 9. My Events

### 9.1 Rolle von My Events

My Events ist der zentrale Verwaltungsbereich für Hosts.

Der Feed ist für Discovery und soziale Interaktion. My Events ist für Planung und Verwaltung.

### 9.2 Ziele von My Events

My Events soll dem User ermöglichen:

- eigene Events zu sehen
- Entwürfe zu verwalten
- veröffentlichte Events zu bearbeiten
- Event-Level zu erweitern
- Teilnehmer zu verwalten
- Eventinformationen zu vervollständigen
- Performance einzusehen
- Events abzusagen oder abzuschließen

### 9.3 My Events Startseite

Die Startseite von My Events sollte Listen oder Cards enthalten:

- Upcoming Events
- Drafts
- Published Events
- Completed Events
- Cancelled Events

Jede Card sollte zeigen:

- Titel
- Datum
- Ort
- Status
- Event-Level
- Teilnehmerzahl
- Completion Score
- Schnellaktionen

### 9.4 Event Management Ansicht

Beim Klick auf ein Event öffnet sich die Management-Ansicht.

Empfohlene Struktur:

1. Overview
2. Details
3. Schedule
4. Location
5. Participants
6. Media
7. Communication
8. Safety
9. Advanced Modules
10. Professional Modules
11. Analytics
12. Settings

Nicht alle Tabs müssen immer sichtbar sein. Sichtbarkeit hängt vom Event-Level und aktivierten Modulen ab.

---

## 10. Event Detail Layer im Feed

### 10.1 Button „Details“

Auf jeder Event-Card im Feed sollte ein Button „Details“ oder „Mehr erfahren“ erscheinen.

### 10.2 Ziel

Der Detail Layer soll mehr Informationen zeigen, ohne den Feed zu überladen.

### 10.3 Varianten

Es gibt zwei mögliche Darstellungsformen:

#### Variante A: Modal / Drawer

Gut für schnelle Nutzung innerhalb der App.

Vorteile:

- schnelle Interaktion
- User bleibt im Feed
- mobile-freundlich
- weniger Kontextwechsel

#### Variante B: eigene Eventseite

Gut für Teilen, SEO, öffentliche Events und Professional Events.

Beispiel:

```text
/events/:slug
```

Empfehlung:

> Kurzfristig Drawer/Modal, langfristig zusätzlich eigene Eventseite.

### 10.4 Inhalte im Detail Layer

Basis:

- Titel
- Bild
- Kurzbeschreibung
- Datum
- Uhrzeit
- Ort
- Host
- Teilnehmerzahl
- Join Button

Advanced:

- lange Beschreibung
- genauer Treffpunkt
- Regeln
- ÖPNV / Parkplatz
- Barrierefreiheit
- Teilnehmerliste optional
- Kontakt

Professional:

- Tickets
- Agenda
- Speaker
- Sponsoren
- Dokumente
- rechtliche Informationen
- Kalenderlinks
- Streaming-Links

---

## 11. Empfehlenswertes Datenmodell

### 11.1 Grundentscheidung

Ein Event sollte nicht komplett getrennt vom Vibe Feed existieren. Stattdessen sollte ein Event eine strukturierte Erweiterung eines Vibe Posts sein.

Empfohlene Kernlogik:

```text
vibes.type = 'event'
events.vibe_id = vibes.id
```

Dadurch kann jedes Event im Feed erscheinen und gleichzeitig strukturierte Eventdaten besitzen.

---

## 12. Datenmodell Übersicht

Empfohlene Tabellen:

- users
- vibes
- events
- event_levels
- event_modules
- venues
- organizers
- event_categories
- event_tags
- tickets
- registrations
- attendees
- sessions
- speakers
- sponsors
- media_assets
- event_media
- event_communications
- event_legal
- event_analytics
- event_integrations
- event_audit_log

---

## 13. Tabelle: vibes

Die Tabelle `vibes` bleibt der Social Feed Layer.

```sql
CREATE TABLE vibes (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    user_id UUID NOT NULL REFERENCES users(id),
    type VARCHAR(30) NOT NULL DEFAULT 'post',
    content TEXT,
    image_url TEXT,
    visibility VARCHAR(30) NOT NULL DEFAULT 'public',
    location_label VARCHAR(255),
    latitude DECIMAL(10, 7),
    longitude DECIMAL(10, 7),
    created_at TIMESTAMP WITH TIME ZONE DEFAULT now(),
    updated_at TIMESTAMP WITH TIME ZONE DEFAULT now(),
    deleted_at TIMESTAMP WITH TIME ZONE
);
```

### 13.1 Vibe Types

Empfohlene Werte:

```text
post
event
moment
question
announcement
```

Für Events gilt:

```text
vibes.type = event
```

---

## 14. Tabelle: events

Die Tabelle `events` enthält die Event-Kerndaten.

```sql
CREATE TABLE events (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    vibe_id UUID UNIQUE REFERENCES vibes(id) ON DELETE CASCADE,
    host_user_id UUID NOT NULL REFERENCES users(id),

    slug VARCHAR(255) UNIQUE NOT NULL,
    title VARCHAR(255) NOT NULL,
    subtitle VARCHAR(255),
    description_short TEXT,
    description_long TEXT,

    event_type VARCHAR(50) DEFAULT 'Sonstiges',
    category_id UUID REFERENCES event_categories(id),

    status VARCHAR(30) NOT NULL DEFAULT 'draft',
    visibility VARCHAR(30) NOT NULL DEFAULT 'public',
    event_level VARCHAR(30) NOT NULL DEFAULT 'basic',

    language VARCHAR(10) DEFAULT 'de',
    timezone VARCHAR(80) DEFAULT 'Europe/Berlin',

    start_datetime TIMESTAMP WITH TIME ZONE NOT NULL,
    end_datetime TIMESTAMP WITH TIME ZONE,
    registration_open TIMESTAMP WITH TIME ZONE,
    registration_close TIMESTAMP WITH TIME ZONE,
    check_in_start TIMESTAMP WITH TIME ZONE,
    doors_open TIMESTAMP WITH TIME ZONE,
    event_duration_minutes INTEGER,
    is_all_day BOOLEAN DEFAULT false,
    is_recurring BOOLEAN DEFAULT false,
    recurrence_pattern TEXT,

    venue_id UUID REFERENCES venues(id),
    is_online BOOLEAN DEFAULT false,
    stream_url TEXT,
    meeting_url TEXT,
    meeting_password TEXT,
    platform VARCHAR(100),
    livestream_provider VARCHAR(100),
    recording_available BOOLEAN DEFAULT false,

    organizer_id UUID REFERENCES organizers(id),

    ticket_required BOOLEAN DEFAULT false,
    max_attendees INTEGER,
    min_attendees INTEGER,
    waitlist_enabled BOOLEAN DEFAULT false,
    currency CHAR(3) DEFAULT 'EUR',
    price_from NUMERIC(10,2),
    price_to NUMERIC(10,2),
    early_bird_enabled BOOLEAN DEFAULT false,
    refund_policy TEXT,
    cancellation_policy TEXT,

    cover_image_url TEXT,
    banner_image_url TEXT,
    video_url TEXT,

    food_available BOOLEAN DEFAULT false,
    drinks_available BOOLEAN DEFAULT false,
    meal_type VARCHAR(100),
    dietary_options TEXT,
    allergen_information TEXT,

    photo_consent_required BOOLEAN DEFAULT false,
    waiver_required BOOLEAN DEFAULT false,
    age_restriction BOOLEAN DEFAULT false,
    minimum_age INTEGER,

    completion_score INTEGER DEFAULT 0,

    created_at TIMESTAMP WITH TIME ZONE DEFAULT now(),
    updated_at TIMESTAMP WITH TIME ZONE DEFAULT now(),
    published_at TIMESTAMP WITH TIME ZONE,
    cancelled_at TIMESTAMP WITH TIME ZONE,
    completed_at TIMESTAMP WITH TIME ZONE,
    deleted_at TIMESTAMP WITH TIME ZONE
);
```

### 14.1 Event Status

Empfohlene Werte:

```text
draft
published
cancelled
completed
archived
```

### 14.2 Event Visibility

Empfohlene Werte:

```text
public
private
invite_only
unlisted
```

### 14.3 Event Level

Empfohlene Werte:

```text
basic
advanced
professional
```

### 14.4 Event Types

Empfohlene Werte:

```text
Konferenz
Meetup
Workshop
Konzert
Webinar
Messe
Festival
Sonstiges
```

---

## 15. Tabelle: event_modules

Event-Level allein reicht langfristig nicht. Zusätzlich sollten einzelne Module aktiviert werden können.

```sql
CREATE TABLE event_modules (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    event_id UUID NOT NULL REFERENCES events(id) ON DELETE CASCADE,
    module_name VARCHAR(80) NOT NULL,
    enabled BOOLEAN DEFAULT true,
    enabled_at TIMESTAMP WITH TIME ZONE DEFAULT now(),
    enabled_by UUID REFERENCES users(id),
    UNIQUE(event_id, module_name)
);
```

### 15.1 Empfohlene Module

```text
agenda
tickets
attendees
waitlist
speakers
sponsors
media_gallery
documents
communication
reminders
check_in
analytics
legal
integrations
catering
online_event
```

### 15.2 Vorteil

Dadurch kann ein Event flexibel wachsen. Ein Advanced Event kann zum Beispiel Tickets deaktiviert lassen, aber Teilnehmerverwaltung nutzen. Ein Professional Event kann Sponsoren haben, aber keine Sessions.

---

## 16. Tabelle: venues

```sql
CREATE TABLE venues (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    created_by UUID REFERENCES users(id),

    name VARCHAR(255) NOT NULL,
    description TEXT,
    address_line_1 VARCHAR(255),
    address_line_2 VARCHAR(255),
    postal_code VARCHAR(30),
    city VARCHAR(120),
    state VARCHAR(120),
    country VARCHAR(120) DEFAULT 'Germany',
    latitude DECIMAL(10,7),
    longitude DECIMAL(10,7),
    room_name VARCHAR(120),
    floor VARCHAR(50),
    capacity INTEGER,
    parking_available BOOLEAN DEFAULT false,
    public_transport_info TEXT,
    accessibility_info TEXT,

    created_at TIMESTAMP WITH TIME ZONE DEFAULT now(),
    updated_at TIMESTAMP WITH TIME ZONE DEFAULT now()
);
```

### 16.1 Empfehlung

Für Basis Events muss kein vollständiger Venue-Datensatz erzwungen werden. Ein freies `location_label` reicht. Erst bei Advanced oder Professional sollte ein strukturierter Venue-Datensatz empfohlen werden.

---

## 17. Tabelle: organizers

```sql
CREATE TABLE organizers (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    owner_user_id UUID REFERENCES users(id),

    name VARCHAR(255) NOT NULL,
    email VARCHAR(255),
    phone VARCHAR(80),
    website TEXT,
    logo_url TEXT,
    description TEXT,

    is_verified BOOLEAN DEFAULT false,
    created_at TIMESTAMP WITH TIME ZONE DEFAULT now(),
    updated_at TIMESTAMP WITH TIME ZONE DEFAULT now()
);
```

### 17.1 Empfehlung

Für Basis Events ist der User selbst der Host. Für Advanced und Professional Events kann ein Organizer-Profil sinnvoll sein.

---

## 18. Tabellen: Kategorien und Tags

### 18.1 event_categories

```sql
CREATE TABLE event_categories (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    name VARCHAR(120) NOT NULL UNIQUE,
    slug VARCHAR(120) NOT NULL UNIQUE,
    description TEXT,
    icon VARCHAR(80),
    color VARCHAR(30),
    created_at TIMESTAMP WITH TIME ZONE DEFAULT now()
);
```

### 18.2 event_tags

```sql
CREATE TABLE event_tags (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    name VARCHAR(120) NOT NULL UNIQUE,
    slug VARCHAR(120) NOT NULL UNIQUE,
    created_at TIMESTAMP WITH TIME ZONE DEFAULT now()
);
```

### 18.3 event_tag_map

```sql
CREATE TABLE event_tag_map (
    event_id UUID NOT NULL REFERENCES events(id) ON DELETE CASCADE,
    tag_id UUID NOT NULL REFERENCES event_tags(id) ON DELETE CASCADE,
    PRIMARY KEY (event_id, tag_id)
);
```

---

## 19. Tabelle: tickets

```sql
CREATE TABLE tickets (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    event_id UUID NOT NULL REFERENCES events(id) ON DELETE CASCADE,

    name VARCHAR(255) NOT NULL,
    description TEXT,
    price NUMERIC(10,2) NOT NULL DEFAULT 0,
    currency CHAR(3) DEFAULT 'EUR',
    quantity INTEGER,
    quantity_sold INTEGER DEFAULT 0,
    sale_start TIMESTAMP WITH TIME ZONE,
    sale_end TIMESTAMP WITH TIME ZONE,
    max_per_order INTEGER DEFAULT 1,
    is_active BOOLEAN DEFAULT true,

    created_at TIMESTAMP WITH TIME ZONE DEFAULT now(),
    updated_at TIMESTAMP WITH TIME ZONE DEFAULT now()
);
```

### 19.1 Empfehlung

Tickets gehören ausschließlich in Professional oder optional in Advanced. Für Basis Events sollte die UI keine Ticketlogik zeigen.

---

## 20. Tabelle: registrations

Die Registrierung ist die Verbindung zwischen User und Event.

```sql
CREATE TABLE registrations (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    event_id UUID NOT NULL REFERENCES events(id) ON DELETE CASCADE,
    user_id UUID REFERENCES users(id),
    ticket_id UUID REFERENCES tickets(id),

    first_name VARCHAR(120),
    last_name VARCHAR(120),
    email VARCHAR(255),
    phone VARCHAR(80),
    company VARCHAR(255),
    job_title VARCHAR(255),
    notes TEXT,

    status VARCHAR(50) NOT NULL DEFAULT 'registered',
    attendance_status VARCHAR(50) DEFAULT 'not_checked_in',
    registration_date TIMESTAMP WITH TIME ZONE DEFAULT now(),
    check_in_time TIMESTAMP WITH TIME ZONE,

    created_at TIMESTAMP WITH TIME ZONE DEFAULT now(),
    updated_at TIMESTAMP WITH TIME ZONE DEFAULT now()
);
```

### 20.1 Registration Status

```text
requested
approved
registered
waitlisted
cancelled
rejected
no_show
checked_in
```

---

## 21. Tabelle: sessions

```sql
CREATE TABLE sessions (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    event_id UUID NOT NULL REFERENCES events(id) ON DELETE CASCADE,
    speaker_id UUID REFERENCES speakers(id),

    title VARCHAR(255) NOT NULL,
    description TEXT,
    start_time TIMESTAMP WITH TIME ZONE,
    end_time TIMESTAMP WITH TIME ZONE,
    room VARCHAR(120),
    capacity INTEGER,
    session_type VARCHAR(80),

    created_at TIMESTAMP WITH TIME ZONE DEFAULT now(),
    updated_at TIMESTAMP WITH TIME ZONE DEFAULT now()
);
```

---

## 22. Tabelle: speakers

```sql
CREATE TABLE speakers (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    event_id UUID REFERENCES events(id) ON DELETE CASCADE,

    first_name VARCHAR(120),
    last_name VARCHAR(120),
    display_name VARCHAR(255) NOT NULL,
    bio TEXT,
    photo_url TEXT,
    website TEXT,
    linkedin_url TEXT,
    twitter_url TEXT,
    company VARCHAR(255),
    position VARCHAR(255),

    created_at TIMESTAMP WITH TIME ZONE DEFAULT now(),
    updated_at TIMESTAMP WITH TIME ZONE DEFAULT now()
);
```

---

## 23. Tabelle: sponsors

```sql
CREATE TABLE sponsors (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    event_id UUID NOT NULL REFERENCES events(id) ON DELETE CASCADE,

    name VARCHAR(255) NOT NULL,
    tier VARCHAR(120),
    website TEXT,
    logo_url TEXT,
    description TEXT,
    contact_email VARCHAR(255),

    created_at TIMESTAMP WITH TIME ZONE DEFAULT now(),
    updated_at TIMESTAMP WITH TIME ZONE DEFAULT now()
);
```

---

## 24. Medienmodell

### 24.1 media_assets

```sql
CREATE TABLE media_assets (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    uploaded_by UUID REFERENCES users(id),

    url TEXT NOT NULL,
    storage_provider VARCHAR(80) DEFAULT 'azure_blob',
    mime_type VARCHAR(120),
    file_size_bytes BIGINT,
    alt_text TEXT,
    caption TEXT,

    created_at TIMESTAMP WITH TIME ZONE DEFAULT now()
);
```

### 24.2 event_media

```sql
CREATE TABLE event_media (
    event_id UUID NOT NULL REFERENCES events(id) ON DELETE CASCADE,
    media_id UUID NOT NULL REFERENCES media_assets(id) ON DELETE CASCADE,
    media_role VARCHAR(80) NOT NULL DEFAULT 'gallery',
    sort_order INTEGER DEFAULT 0,
    PRIMARY KEY (event_id, media_id, media_role)
);
```

### 24.3 Media Roles

```text
cover
banner
gallery
video
document
attachment
organizer_logo
sponsor_logo
speaker_photo
```

---

## 25. Tabelle: event_communications

```sql
CREATE TABLE event_communications (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    event_id UUID NOT NULL REFERENCES events(id) ON DELETE CASCADE,

    confirmation_email_template TEXT,
    reminder_email_template TEXT,
    thank_you_email_template TEXT,
    notification_settings JSONB,
    contact_email VARCHAR(255),
    contact_phone VARCHAR(80),

    created_at TIMESTAMP WITH TIME ZONE DEFAULT now(),
    updated_at TIMESTAMP WITH TIME ZONE DEFAULT now()
);
```

---

## 26. Tabelle: event_legal

```sql
CREATE TABLE event_legal (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    event_id UUID NOT NULL REFERENCES events(id) ON DELETE CASCADE,

    terms_url TEXT,
    privacy_policy_url TEXT,
    imprint_url TEXT,
    photo_consent_required BOOLEAN DEFAULT false,
    waiver_required BOOLEAN DEFAULT false,
    age_restriction BOOLEAN DEFAULT false,
    minimum_age INTEGER,

    created_at TIMESTAMP WITH TIME ZONE DEFAULT now(),
    updated_at TIMESTAMP WITH TIME ZONE DEFAULT now()
);
```

---

## 27. Tabelle: event_analytics

```sql
CREATE TABLE event_analytics (
    event_id UUID PRIMARY KEY REFERENCES events(id) ON DELETE CASCADE,

    page_views INTEGER DEFAULT 0,
    registrations INTEGER DEFAULT 0,
    attendees_count INTEGER DEFAULT 0,
    check_ins_count INTEGER DEFAULT 0,
    ticket_revenue NUMERIC(12,2) DEFAULT 0,
    conversion_rate NUMERIC(6,4),

    updated_at TIMESTAMP WITH TIME ZONE DEFAULT now()
);
```

### 27.1 Empfehlung

Für MVP reichen einfache aggregierte Werte. Später können Event-Tracking-Daten zusätzlich in separaten Event-Tracking-Tabellen gespeichert werden.

---

## 28. Tabelle: event_integrations

```sql
CREATE TABLE event_integrations (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    event_id UUID NOT NULL REFERENCES events(id) ON DELETE CASCADE,

    google_calendar_url TEXT,
    ical_url TEXT,
    zoom_meeting_id VARCHAR(255),
    youtube_stream_id VARCHAR(255),
    stripe_product_id VARCHAR(255),
    paypal_product_id VARCHAR(255),

    created_at TIMESTAMP WITH TIME ZONE DEFAULT now(),
    updated_at TIMESTAMP WITH TIME ZONE DEFAULT now()
);
```

---

## 29. Tabelle: event_audit_log

```sql
CREATE TABLE event_audit_log (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    event_id UUID NOT NULL REFERENCES events(id) ON DELETE CASCADE,
    actor_user_id UUID REFERENCES users(id),

    action VARCHAR(120) NOT NULL,
    old_value JSONB,
    new_value JSONB,
    metadata JSONB,

    created_at TIMESTAMP WITH TIME ZONE DEFAULT now()
);
```

### 29.1 Zweck

Der Audit Log ist wichtig für:

- Moderation
- Sicherheit
- spätere Admin-Tools
- Nachvollziehbarkeit
- Professional Events
- Streitfälle bei Tickets oder Absagen

---

## 30. Completion Score

### 30.1 Idee

Jedes Event erhält einen Completion Score. Dieser zeigt dem Host, wie vollständig das Event eingerichtet ist.

Beispiel:

```text
Basis vollständig: 100%
Advanced: 45%
Professional: 10%
```

### 30.2 Warum sinnvoll

Der Completion Score motiviert den User, sein Event zu verbessern, ohne ihn zu zwingen.

### 30.3 Beispiel-Logik

Basis:

- Titel vorhanden
- Datum vorhanden
- Ort oder Online vorhanden
- Kurzbeschreibung vorhanden
- Bild vorhanden

Advanced:

- lange Beschreibung vorhanden
- Teilnehmerlimit gesetzt
- genauer Treffpunkt vorhanden
- Kontaktinfo vorhanden
- Reminder aktiviert
- Regeln ergänzt

Professional:

- Tickets eingerichtet
- Agenda vorhanden
- Speaker vorhanden
- Legal-Infos vorhanden
- Analytics aktiv
- Integrationen eingerichtet

---

## 31. API-Konzept

### 31.1 Feed APIs

```http
GET /api/vibes
POST /api/vibes
GET /api/vibes/:id
PATCH /api/vibes/:id
DELETE /api/vibes/:id
```

### 31.2 Event APIs

```http
GET /api/events
POST /api/events
GET /api/events/:id
GET /api/events/slug/:slug
PATCH /api/events/:id
DELETE /api/events/:id
```

### 31.3 My Events APIs

```http
GET /api/me/events
GET /api/me/events/upcoming
GET /api/me/events/drafts
GET /api/me/events/published
GET /api/me/events/completed
PATCH /api/me/events/:id
```

### 31.4 Upgrade APIs

```http
POST /api/events/:id/upgrade
POST /api/events/:id/modules/:moduleName/enable
POST /api/events/:id/modules/:moduleName/disable
```

Beispiel Payload:

```json
{
  "event_level": "advanced",
  "modules": ["attendees", "reminders", "waitlist"]
}
```

### 31.5 Registrations APIs

```http
POST /api/events/:id/register
POST /api/events/:id/join
DELETE /api/events/:id/registration
GET /api/events/:id/registrations
PATCH /api/events/:id/registrations/:registrationId
```

### 31.6 Tickets APIs

```http
GET /api/events/:id/tickets
POST /api/events/:id/tickets
PATCH /api/events/:id/tickets/:ticketId
DELETE /api/events/:id/tickets/:ticketId
```

### 31.7 Sessions APIs

```http
GET /api/events/:id/sessions
POST /api/events/:id/sessions
PATCH /api/events/:id/sessions/:sessionId
DELETE /api/events/:id/sessions/:sessionId
```

---

## 32. Frontend Roadmap

### 32.1 Phase 1: Feed Event Creation

Ziel:

Ein User kann schnell einen Event-Vibe erstellen.

Features:

- Event Toggle im Create Vibe Formular
- Eventname
- kurzer Text
- Datum/Uhrzeit
- Ort
- Bild
- Sichtbarkeit
- Veröffentlichung im Feed
- Basic Event Datensatz im Backend

### 32.2 Phase 2: Event Card im Feed

Ziel:

Events sind im Feed klar erkennbar, aber nicht überladen.

Features:

- Event-Badge
- Datum/Uhrzeit
- Ort
- Hosting Label
- Join Button
- Details Button
- Teilnehmerzahl
- Statusanzeige

### 32.3 Phase 3: Event Detail Drawer

Ziel:

Mehr Informationen ohne Feed-Überladung.

Features:

- Drawer oder Modal
- Basisinformationen
- Host-Karte
- Join-Funktion
- Teilen
- Kalender hinzufügen
- Map / Ort

### 32.4 Phase 4: My Events Übersicht

Ziel:

User kann eigene Events verwalten.

Features:

- linkes Menü „My Events“
- Eventlisten
- Filter nach Status
- Event-Level sichtbar
- Completion Score
- Schnellaktionen

### 32.5 Phase 5: Event Editor Basis

Ziel:

Basis Events können bearbeitet werden.

Features:

- Titel ändern
- Kurzbeschreibung ändern
- Datum ändern
- Ort ändern
- Bild ändern
- Sichtbarkeit ändern
- Teilnehmerlimit setzen
- Event veröffentlichen / zurück auf Draft
- Event absagen

### 32.6 Phase 6: Event erweitern

Ziel:

User kann ein Event upgraden.

Features:

- Button „Event erweitern“
- Auswahl Advanced / Professional
- Erklärung der Vorteile
- Aktivierung von Modulen
- keine Datenverluste
- UI passt sich an

### 32.7 Phase 7: Advanced Event Management

Ziel:

Community-Events können sauber geplant werden.

Features:

- lange Beschreibung
- genauer Treffpunkt
- Teilnehmerverwaltung
- Warteliste
- Reminder
- Regeln
- Kontaktinfos
- Barrierefreiheit
- ÖPNV / Parken
- Wiederholungen

### 32.8 Phase 8: Professional Event Management

Ziel:

Große Events können professionell organisiert werden.

Features:

- Tickets
- Preislogik
- Sessions
- Speaker
- Sponsoren
- Dokumente
- Mediengalerie
- Legal Informationen
- Analytics
- Integrationen

---

## 33. Backend Roadmap

### 33.1 Phase 1: Datenbankgrundlage

- vibes.type erweitern
- events Tabelle erstellen
- Beziehung vibe_id zu events
- Basisstatus und Visibility
- Slug-Generierung
- Host-Zuordnung

### 33.2 Phase 2: Event APIs

- Create Basic Event
- Update Event
- Get Event
- Get My Events
- Publish / Cancel / Complete

### 33.3 Phase 3: Registration System

- Join Event
- Leave Event
- Teilnehmer zählen
- Teilnehmerliste für Host
- Max Attendees prüfen
- Waitlist vorbereiten

### 33.4 Phase 4: Module System

- event_modules Tabelle
- Upgrade API
- Modulaktivierung
- Feature Guards im Backend

### 33.5 Phase 5: Advanced Models

- venues
- organizers
- event_tags
- event_categories
- event_communications

### 33.6 Phase 6: Professional Models

- tickets
- sessions
- speakers
- sponsors
- event_media
- event_legal
- event_integrations
- event_analytics

### 33.7 Phase 7: Safety & Moderation

- Report Event
- Host Trust Signals
- Admin Review
- Audit Log
- automatische Warnungen bei sensiblen Events

---

## 34. Sicherheits- und Trust-Konzept

Da nVibes reale Treffen ermöglicht, ist Sicherheit zentral.

### 34.1 Event Trust Signals

Event Cards und Detailseiten sollten langfristig anzeigen:

- verifizierter Host
- Trust Score des Hosts
- öffentlicher Treffpunkt
- Teilnehmeranzahl
- gemeinsame Kontakte
- Eventhistorie des Hosts
- Report Button
- Sicherheitsinformationen

### 34.2 Sicherheitsfelder

Mögliche Felder:

- is_public_place
- safety_notes
- minimum_age
- age_restriction
- parent_approval_required
- verified_host_required
- report_count
- moderation_status

### 34.3 Moderation Status

```text
pending_review
approved
flagged
restricted
removed
```

---

## 35. Datenschutz und Sichtbarkeit

### 35.1 Public Events

Öffentlich sichtbar. Können im Feed und eventuell in der Suche erscheinen.

### 35.2 Private Events

Nur für ausgewählte User sichtbar.

### 35.3 Invite Only Events

Nur per Einladung sichtbar oder beitretbar.

### 35.4 Unlisted Events

Nicht in Discovery sichtbar, aber über Link erreichbar.

---

## 36. Rollenmodell

### 36.1 Eventrollen

```text
host
co_host
moderator
speaker
sponsor
attendee
waitlisted
invited
```

### 36.2 Empfohlene Tabelle: event_roles

```sql
CREATE TABLE event_roles (
    id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
    event_id UUID NOT NULL REFERENCES events(id) ON DELETE CASCADE,
    user_id UUID NOT NULL REFERENCES users(id),
    role VARCHAR(50) NOT NULL,
    created_at TIMESTAMP WITH TIME ZONE DEFAULT now(),
    UNIQUE(event_id, user_id, role)
);
```

---

## 37. Naming und UI-Sprache

### 37.1 Empfohlene Begriffe

| Funktion | Empfohlener Begriff |
|---|---|
| Details öffnen | Details |
| Event ausbauen | Event erweitern |
| Basic Level | Basis |
| Advanced Level | Advanced |
| Professional Level | Professional |
| Teilnehmer | People / Teilnehmer |
| Hostbereich | My Events |
| Beitreten | Join / Teilnehmen |

### 37.2 Tonalität

nVibes sollte nicht bürokratisch klingen.

Besser:

> „Mach dein Event größer.“

Statt:

> „Aktivieren Sie zusätzliche Verwaltungsfunktionen.“

Besser:

> „Füge mehr Details hinzu, damit andere wissen, was sie erwartet.“

Statt:

> „Bitte vervollständigen Sie die Eventdaten.“

---

## 38. MVP-Empfehlung

Für den ersten produktiven Schritt sollte nicht das gesamte Professional-System gebaut werden.

### 38.1 MVP Scope

MVP sollte beinhalten:

- Event-Vibe erstellen
- Event im Feed anzeigen
- Details Button
- Event Detail Drawer
- Join / Leave
- My Events Übersicht
- Basis Event bearbeiten
- Status: Draft, Published, Cancelled, Completed
- Event-Level Feld vorbereiten
- Completion Score einfach vorbereiten

### 38.2 Noch nicht im MVP

- Tickets
- Payments
- Sponsoren
- Speaker
- komplexe Agenda
- Analytics Dashboard
- Integrationen
- umfangreiche Legal-Module

Diese Funktionen sollten strukturell vorbereitet, aber nicht sofort vollständig umgesetzt werden.

---

## 39. Empfohlene Entwicklungsreihenfolge

### Schritt 1

Datenmodell für `events` mit `vibe_id` einführen.

### Schritt 2

Create Vibe Flow um Event-Felder erweitern.

### Schritt 3

Feed Card für Event-Vibes anpassen.

### Schritt 4

Event Detail Drawer entwickeln.

### Schritt 5

My Events Übersicht entwickeln.

### Schritt 6

Basis Event Editor entwickeln.

### Schritt 7

Join / Registration System entwickeln.

### Schritt 8

Upgrade Flow vorbereiten.

### Schritt 9

Advanced Module implementieren.

### Schritt 10

Professional Module schrittweise ergänzen.

---

## 40. Zukunftsperspektiven

### 40.1 Event Discovery

Langfristig kann nVibes intelligente Event Discovery anbieten:

- Nearby Events
- Interessenbasierte Events
- Freunde gehen hin
- Wiederkehrende Community Events
- Uni / Campus Events
- sichere öffentliche Treffpunkte

### 40.2 Social Graph Integration

Events können stärker mit dem sozialen Graphen verbunden werden:

- Freunde nehmen teil
- Freunde hosten
- ähnliche Vibes
- gemeinsame Interessen
- Gruppenbasierte Events

### 40.3 Badges und Challenges

Events sind ideal für das Badge-System.

Mögliche Badges:

- First Event Host
- Coffee Connector
- Community Builder
- Trusted Organizer
- Local Explorer
- Safe Host
- Event Organizer
- City Connector

### 40.4 Trust-basierte Eventqualität

Langfristig können Events priorisiert werden nach:

- Host Trust
- Teilnehmerfeedback
- Eventhistorie
- Sicherheitslevel
- öffentlichen Orten
- Community-Relevanz

### 40.5 Professionelle Monetarisierung

Professional Events können später ein Geschäftsmodell ermöglichen:

- Ticketgebühren
- Organizer-Abos
- Featured Events
- Community Tools
- Analytics für Veranstalter
- Premium Organizer Profile

Wichtig: Monetarisierung darf nicht die nVibes-DNA zerstören. Die Plattform sollte weiterhin echte Begegnungen und menschliche Verbindung priorisieren.

---

## 41. Strategische Empfehlung

Das Eventmanagement sollte als skalierbares System gebaut werden, aber in der UX extrem leicht bleiben.

Die wichtigste Produktregel lautet:

> Der erste Event-Post muss einfach bleiben. Die Komplexität gehört nach My Events.

Das schützt die nVibes-DNA.

nVibes sollte nicht mit Eventbrite konkurrieren, indem es ein weiteres Formularsystem baut. nVibes sollte Events so denken:

> Aus einem spontanen sozialen Moment kann ein echtes Event werden.

Das ist die besondere Stärke.

---

## 42. Finale Architektur-Empfehlung

### 42.1 Kurzform

- `vibes` bleibt der Social Layer.
- `events` erweitert Vibes zu strukturierten Events.
- `event_level` steuert Basis, Advanced, Professional.
- `event_modules` steuert flexible Funktionen.
- `My Events` wird der Verwaltungsbereich.
- Der Feed bleibt clean.
- Details werden über Drawer oder Eventseite angezeigt.
- Professional Features werden modular nachgerüstet.

### 42.2 Leitbild für die Entwicklung

> Build simple at the surface, powerful underneath.

Oder auf Deutsch:

> Für den User einfach. Unter der Haube professionell.

---

## 43. Dev-Line für LLM-gestützte Entwicklung

Dieses Dokument dient als Entwicklungsleitfaden. Bei späteren Entwicklungsaufgaben sollte die LLM folgende Prinzipien beachten:

1. Keine Überladung des Feed-Create-Flows.
2. Events sind spezielle Vibes, keine isolierten Fremdkörper.
3. My Events ist der Ort für Komplexität.
4. Basis Events müssen immer schnell erstellbar bleiben.
5. Advanced und Professional sind Erweiterungen, keine Pflicht.
6. Upgrades dürfen keine Daten löschen.
7. Module sollten flexibel aktiviert werden können.
8. Sicherheit und Vertrauen sind zentrale Eventbestandteile.
9. Die Datenbank soll langfristig Professional Events ermöglichen.
10. MVP-Fokus liegt auf Erstellung, Anzeige, Details, My Events und Join.
11. Tickets, Speaker, Sponsoren und Analytics kommen später.
12. Jede UX-Entscheidung muss zur nVibes-Idee passen: echte Begegnungen, geringe Hürde, menschliche Verbindung.

---

## 44. Abschluss

Das geplante Eventmanagement kann zu einem der wichtigsten Kernbereiche von nVibes werden.

Es verbindet:

- Social Feed
- spontane Treffen
- lokale Discovery
- Community Building
- sichere reale Begegnungen
- spätere professionelle Eventverwaltung

Die beste Umsetzung ist kein klassisches Eventformular, sondern ein wachsendes Eventsystem:

```text
Vibe posten → Event entsteht → Details ansehen → My Events bearbeiten → Event erweitern → Community wächst
```

Damit bleibt nVibes spontan, menschlich und modern, kann aber langfristig zu einer echten Social Infrastructure for Real Human Connection werden.
