# iOSHowTos

## Table of contents

[#1 How to change color of navigation bar in SwiftUI?](https://github.com/bnulo/ioshowtos#how-to-change-color-of-navigation-bar-in-swiftui?)


class MentionDetectorTests: XCTestCase {
    func testDetectingMention() {
        let detector = MentionDetector()
        let string = "This test was written by @johnsundell."

        detector.detectMentions(in: string) { mentions in
            XCTAssertEqual(mentions, ["johnsundell"])
        }
        
        sleep(2)
    }
}

// AFTER:

class MentionDetectorTests: XCTestCase {
    func testDetectingMention() {
        let detector = MentionDetector()
        let string = "This test was written by @johnsundell."

        var mentions: [String]?
        let expectation = self.expectation(description: #function)

        detector.detectMentions(in: string) {
            mentions = $0
            expectation.fulfill()
        }

        waitForExpectations(timeout: 10)
        XCTAssertEqual(mentions, ["johnsundell"])
    }
}
class MentionDetectorTests: XCTestCase {
    func testDetectingMention() {
        let detector = MentionDetector()
        let string = "This test was written by @johnsundell."

        detector.detectMentions(in: string) { mentions in
            XCTAssertEqual(mentions, ["johnsundell"])
        }
        
        sleep(2)
    }
}

// AFTER:

class MentionDetectorTests: XCTestCase {
    func testDetectingMention() {
        let detector = MentionDetector()
        let string = "This test was written by @johnsundell."

        var mentions: [String]?
        let expectation = self.expectation(description: #function)

        detector.detectMentions(in: string) {
            mentions = $0
            expectation.fulfill()
        }

        waitForExpectations(timeout: 10)
        XCTAssertEqual(mentions, ["johnsundell"])
    }
}
class MentionDetectorTests: XCTestCase {
    func testDetectingMention() {
        let detector = MentionDetector()
        let string = "This test was written by @johnsundell."

        detector.detectMentions(in: string) { mentions in
            XCTAssertEqual(mentions, ["johnsundell"])
        }
        
        sleep(2)
    }
}

// AFTER:

class MentionDetectorTests: XCTestCase {
    func testDetectingMention() {
        let detector = MentionDetector()
        let string = "This test was written by @johnsundell."

        var mentions: [String]?
        let expectation = self.expectation(description: #function)

        detector.detectMentions(in: string) {
            mentions = $0
            expectation.fulfill()
        }

        waitForExpectations(timeout: 10)
        XCTAssertEqual(mentions, ["johnsundell"])
    }
}
class MentionDetectorTests: XCTestCase {
    func testDetectingMention() {
        let detector = MentionDetector()
        let string = "This test was written by @johnsundell."

        detector.detectMentions(in: string) { mentions in
            XCTAssertEqual(mentions, ["johnsundell"])
        }
        
        sleep(2)
    }
}

// AFTER:

class MentionDetectorTests: XCTestCase {
    func testDetectingMention() {
        let detector = MentionDetector()
        let string = "This test was written by @johnsundell."

        var mentions: [String]?
        let expectation = self.expectation(description: #function)

        detector.detectMentions(in: string) {
            mentions = $0
            expectation.fulfill()
        }

        waitForExpectations(timeout: 10)
        XCTAssertEqual(mentions, ["johnsundell"])
    }
}
class MentionDetectorTests: XCTestCase {
    func testDetectingMention() {
        let detector = MentionDetector()
        let string = "This test was written by @johnsundell."

        detector.detectMentions(in: string) { mentions in
            XCTAssertEqual(mentions, ["johnsundell"])
        }
        
        sleep(2)
    }
}

// AFTER:

class MentionDetectorTests: XCTestCase {
    func testDetectingMention() {
        let detector = MentionDetector()
        let string = "This test was written by @johnsundell."

        var mentions: [String]?
        let expectation = self.expectation(description: #function)

        detector.detectMentions(in: string) {
            mentions = $0
            expectation.fulfill()
        }

        waitForExpectations(timeout: 10)
        XCTAssertEqual(mentions, ["johnsundell"])
    }
}
class MentionDetectorTests: XCTestCase {
    func testDetectingMention() {
        let detector = MentionDetector()
        let string = "This test was written by @johnsundell."

        detector.detectMentions(in: string) { mentions in
            XCTAssertEqual(mentions, ["johnsundell"])
        }
        
        sleep(2)
    }
}

// AFTER:

class MentionDetectorTests: XCTestCase {
    func testDetectingMention() {
        let detector = MentionDetector()
        let string = "This test was written by @johnsundell."

        var mentions: [String]?
        let expectation = self.expectation(description: #function)

        detector.detectMentions(in: string) {
            mentions = $0
            expectation.fulfill()
        }

        waitForExpectations(timeout: 10)
        XCTAssertEqual(mentions, ["johnsundell"])
    }
}
class MentionDetectorTests: XCTestCase {
    func testDetectingMention() {
        let detector = MentionDetector()
        let string = "This test was written by @johnsundell."

        detector.detectMentions(in: string) { mentions in
            XCTAssertEqual(mentions, ["johnsundell"])
        }
        
        sleep(2)
    }
}

// AFTER:

class MentionDetectorTests: XCTestCase {
    func testDetectingMention() {
        let detector = MentionDetector()
        let string = "This test was written by @johnsundell."

        var mentions: [String]?
        let expectation = self.expectation(description: #function)

        detector.detectMentions(in: string) {
            mentions = $0
            expectation.fulfill()
        }

        waitForExpectations(timeout: 10)
        XCTAssertEqual(mentions, ["johnsundell"])
    }
}
## How to change color of navigation bar in SwiftUI?

```swift
// BEFORE:

class MentionDetectorTests: XCTestCase {
    
}

// AFTER:

class MentionDetectorTests: XCTestCase {
    
}
```
